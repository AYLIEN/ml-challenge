## Hello

Hello, thank you for taking this challenge. The goal here is to get a sense of your understanding of designing and deploying ML models. We are not looking for the perfect solution as that would definitely require a lot of time and effort, rather we are looking for cues to the depth of your understanding. We would appreciate it if you would help us in that by providing us with comments and explanations behind what you did so we understand your thought process.

If you have any questions then please get in touch sooner rather than later. We wish you all the best and good luck!

**Note:** Please do not create pull request to this PR. Create your own GitHub repository instead and share the link with us.

## Challenge

You are asked to evaluate and deploy a text classifier. The model should be deployed locally as a HTTP service. More details on the API is provided below, and you can find the specification in [prediction-openapi.yaml](./prediction-openapi.yaml).

The language you should use is Python 3.8+, however the framework for ML or API creation is up to you. Please provide instructions for running your project.

You are provided with the following:

* A small text dataset, with training data and test data in the files [train.jsonl.gz](./train.jsonl.gz). and [test.jsonl.gz](./test.jsonl.gz) respectively.
    * The text is in English, and is from a collection of posts to newsgroups on various topics.
    * There are 6 labels: `"space", "electronics", "cryptography", "politics", "hockey", "baseball"`.
    * Each line contains a single example encoded as a JSON object: `{"text": "foo content", "label": "foo label"}`.

* A text classifier created using scikit-learn, in the file `model.py`.
    * You can install the necessary dependencies for the model into your local environment by running `pip install -r requirements.txt`.
    * When executed, this Python module will train a classifier and output a prediction for a single test example to standard output.

You are required to:

1. Provide an appropriate evaluation of the model performance on the test data.
2. Implement a way to persist the trained model to local disk.
3. Implement an API according to the open api specification.
4. Create a web service (in Python 3) to serve the persisted model.
5. Deploy the model locally.
6. Create a container with your solution that can be run on Kubernetes.
7. Provide some sample curl commands or a [Postman](https://www.postman.com/) collection.
8. *Stretch Goal 1* - Suggest and/or implement improvements to the model.
9. *Stretch Goal 2* - Testing of the API before deployment.
10. *Stretch Goal 3* - Metrics API for inspecting current metrics of the service.

**Note:** We expect a web service that can run indefinitely, linearly scale and process as many requests as possible until stopped. The service should be able to accept as many requests as the model can process.