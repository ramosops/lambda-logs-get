# AWS CloudWatch Log Query and Slack Notification

A Python-based AWS Lambda function that queries a log group in AWS CloudWatch, performs a conditional check, and sends a GET request to a specified URL.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Configuration](#configuration)
- [Deployment](#deployment)
- [Contributing](#contributing)

## Features

- Executes a custom query on an AWS CloudWatch log group
- Performs a conditional check on the query results
- Send a GET request to a specified URL

## Requirements

- An AWS account with access to Lambda and CloudWatch services
- Python 3.x
- Request layer added to the Lambda function


## Configuration

To use this code, you need to update some variable values in the source file:

1. Set the `URL` variable to your GET request URL.
2. Set the `LOG_GROUP_NAME` variable to the name of the AWS CloudWatch log group you want to query.
3. Set the `QUERY` variable to the specific query you want to execute on the log group.
4. Modify the conditional check in the source code as needed for your use case.


## Deployment

Follow these steps to deploy the Lambda function:

1. Create a Lambda function in the AWS Management Console or using the AWS CLI.
2. Upload the source code, either by zipping the files and uploading through the console, or using the AWS CLI.
3. Set the Lambda function handler, runtime, and other configurations as needed.
4. Add the necessary layers, such as the Request layer, to the Lambda function.
5. Add necessary triggers, such as CloudWatch events or other AWS services, to invoke the Lambda function.
6. Test the Lambda function to ensure it is working as expected.

## Contributing

Contributions are welcome. To contribute, please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request
