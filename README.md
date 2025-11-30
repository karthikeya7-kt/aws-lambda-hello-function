# AWS Lambda Hello Function

This is a simple serverless function built using **AWS Lambda** and exposed using **API Gateway**.

## What this function does
- Returns a `Hello from Lambda!` message
- Triggered using HTTP API Gateway
- Fully serverless (no servers, no EC2, no VPC required)

## Technologies Used
- AWS Lambda
- AWS API Gateway
- Python 3.9

## Steps I Performed
1. Created a Lambda function from AWS Console  
2. Added code directly inside the console  
3. Deployed the function  
4. Tested using Lambda test event  
5. Created an HTTP API Gateway trigger  
6. Verified output using the public endpoint

## Architecture
       ┌─────────────────────────────┐
       │         Client/User         │
       │  (Browser / Postman / App)  │
       └──────────────┬──────────────┘
                      │  HTTP Request
                      ▼
       ┌─────────────────────────────┐
       │     Amazon API Gateway      │
       │ - Receives HTTP request     │
       │ - Routes to Lambda Function │
       └──────────────┬──────────────┘
                      │  Invoke
                      ▼
       ┌─────────────────────────────┐
       │       AWS Lambda            │
       │ - Executes your Python code │
       │ - Returns JSON Response     │
       └──────────────┬──────────────┘
                      │ Response
                      ▼
       ┌─────────────────────────────┐
       │         Client/User         │
       │ Displays "Hello from Lambda"│
       └─────────────────────────────┘
## What I Built
A simple serverless application where an API Gateway endpoint triggers an AWS Lambda function written in Python. The project demonstrates deploying, testing, and exposing a Lambda function through a public HTTP API. Includes screenshots and demo video.

## Screenshots
created lambda function https://github.com/karthikeya7-kt/aws-lambda-hello-function/blob/main/Screenshot%202025-11-29%20151721.png
simple python code https://github.com/karthikeya7-kt/aws-lambda-hello-function/blob/main/Screenshot%202025-11-29%20151831.png
code tested https://github.com/karthikeya7-kt/aws-lambda-hello-function/blob/main/Screenshot%202025-11-29%20151812.png
triggered api link https://github.com/karthikeya7-kt/aws-lambda-hello-function/blob/main/Screenshot%202025-11-29%20151643.png
resulu appeared on web by using api link https://github.com/karthikeya7-kt/aws-lambda-hello-function/blob/main/Screenshot%202025-11-29%20151628.png
## Demo Video
demo part 1
https://github.com/karthikeya7-kt/aws-lambda-hello-function/blob/main/lambda%201.mp4
demo part 2
https://github.com/karthikeya7-kt/aws-lambda-hello-function/blob/main/lambda%202.mp4






