## Hello

Hello, thank you for taking this challenge. The goal here is to get a sense of your understanding of designing and deploying ML models. We are not looking for the perfect solution as that would definitely require a lot of time and effort, rather we are looking for cues to the depth of your understanding. We would appreciate it if you would help us in that by providing us with comments and explanations behind what you did so we understand your thought process.

Wish you all the best and good luck!

**Note:** This repository is archived to avoid pull-requests, since pull-requests will be public. Please create your own GitHub repository instead and share the link with us.

## Challenge

We are looking to design and deploy a prediction API for news articles. The HTTP endpoint for predicting should be accessible locally. More details on the API is provided below, and you can find the specification in [prediction-openapi.yaml](./prediction-openapi.yaml).

The language you should use is Python 3.x, however the framework for ML or API creation is up to you. Please provide instructions for running your project.

In short, these are the steps you need to implement:

1. The training and deployment of the model based on the dataset `news.csv`
2. An API according to the open api specification
3. A web service implemented in Python 3 integrated with the prediction python module
4. Changes in `docker-compose.yaml` to build the docker image with required ML libraries
5. Provide some sample curl commands or a [Postman](https://www.postman.com/) collection
6. *Stretch Goal 1* - Testing of the API before deployment
7. *Stretch Goal 2* - Metrics API for inspecting current metrics of the service

There is no "strict" validation of your request messages, we mostly care about how you will integrate such transformation into your code.

Please note that we expect a web service that can run indefinitely, linearly scale and process as many requests as possible until stopped. The service should be able to accept as many requests as the model can process.