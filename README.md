#Quick proof of concept for Heroku PHP + Nginx + Memcahed + libmcrypt + new relic buildpack

buildpack is found here: https://github.com/headcanon/heroku-buildpack-php-nginx.git

steps to get going:

    git clone __URL__
    cd __DIR__
    heroku create -b https://github.com/headcanon/heroku-buildpack-php-nginx.git
    git push heroku master

`conf/etc.d` contains the newrelic config file to get going. 

All you have to do is enable the extension via the heroku GUI or

    heroku addons:add newrelic:standard

have fun!

