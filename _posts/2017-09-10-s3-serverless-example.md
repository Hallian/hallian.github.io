---
layout: post
title:  "Serverless SPA on AWS"
date:   2017-09-10
excerpt: "Since serverless applications are all the rage at the moment, I decided to create an example repository to demonstrate how to set it up."
image: "/images/2017-09-10-s3-serverless-example/s3-serverless-example.png"
---

Since serverless applications are all the rage at the moment, I decided to create an example repository to demonstrate how to set it up.

The example consists of a simple React based ToDo application hosted on Amazon S3 via static site hosting. The HTTP Rest backend is implemented with AWS Lambda functions served via AWS ApiGateway. Data is stored on AWS DynamoDB. All of this is set up with CloudFormation templates.

Note that even though this is called a "serverless" architecture there are servers running that host the code. It's only serverless from the developers standpoint. The servers are ran and managed by AWS.

See my [s3-serverless-example <i class="icon fa-github"></i>](https://github.com/Hallian/s3-serverless-example) repository on GitHub for more.