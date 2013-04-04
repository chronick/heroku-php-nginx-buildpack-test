#Quick proof of concept for Heroku PHP + Nginx + Memcahed + libmcrypt + new relic buildpack

buildpack is found here: https://github.com/headcanon/heroku-buildpack-php-nginx.git

steps to get going:

    git clone https://github.com/headcanon/heroku-php-nginx-buildpack-test.git
    cd heroku-php-nginx-buildpack-test
    heroku create -b https://github.com/headcanon/heroku-buildpack-php-nginx.git
    git push heroku master


##New Relic
`conf/etc.d` contains the newrelic config file to get started with the New Relic extension. 

All you have to do is enable the extension via the heroku GUI or

    heroku addons:add newrelic:standard

have fun!

