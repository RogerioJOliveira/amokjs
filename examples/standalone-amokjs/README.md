# amokjs - standalone example

Simple example of using [amokjs](https://github.com/sauliuz/amokjs) as a standalone backend mock application. Mocked API responses are served from `responses` directory.

## how to run

    npm install
    node app.js

## test local mock

Few example curl requests to test the local mock API

    curl -XGET 'http://localhost:3000/xml'
    curl -XGET -H 'x-mock-filename: xml' 'http://localhost:3000/'
    curl -XGET -H "x-mock-response-code: 500" 'http://localhost:3000/xml'
