Example oauth2orize Consumer
===

This is an oauth2 consumer that uses `passport-oauth` and `passport-oauth2` to communicate with any oauth2 provider.

Forked from [example-oauth2orize-consumer](https://github.com/coolaj86/example-oauth2orize-consumer) with the following changes:
* Config set in provider-config.js and oauth-config.js
* Uses example-oauth2orize-consumer strategy
* Include process.env.NODE_TLS_REJECT_UNAUTHORIZED = '0' so non-trusted SSL certificates are not rejected (See [here](http://stackoverflow.com/questions/18461979/node-js-error-with-ssl-unable-to-verify-leaf-signature))

Installation
===

    npm install -g jade

    git clone https://github.com/chico/example-oauth2orize-consumer.git
    pushd example-oauth2orize-consumer/
    npm install
    jade public/*.jade

Usage
===

    node ./server 3001

Then visit <http://localhost:3001> and play around.

Config
===

Edit `./provider-config.js` and `./oauth-config.js` to point to your desired oauth2 provider and set the client id and secret.
