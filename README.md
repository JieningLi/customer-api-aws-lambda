# Build a serverless RESTful customer API with Node.js and AWS Lambda

This project demonstrates how to setup a RESTful Web Services allowing you to create, list, get, update and delete customers. DynamoDB is used to store the data.

## Prerequisites

- Node.js v12.x or greater
- An AWS account. You can sign up for a free account [here](http://aws.amazon.com/free)

## Built With

- [AWS Lambda](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
- [Node.js](nodejs.org)

## Endpoints

POST - your.domain.name/dev/customers

GET - your.domain.name/dev/customers

GET - your.domain.name/dev/customers/{id}

DELETE - your.domain.name/dev/customers/{id}

## Run project

- Install the serverless framework: `npm install -g serverless`

- Deploy: `serverless deploy`

  (You will need to configure the serverless CLI with your AWS credentials; please follow [this instruction](https://www.youtube.com/watch?v=HSd9uYj2LJA))

## Run test

Before you can run tests, you need to set the CUSTOMERS_ENDPOINT environment variable to the value of the domain name returned when you deployed your service. Using values from the example above:

- `export CUSTOMERS_ENDPOINT=your.domain.name/dev`

- `npm test`
