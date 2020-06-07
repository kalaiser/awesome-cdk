---
title: Awesome CDK
site_description: A curated list of awesome projects related to the AWS Cloud Development Kit
ogimage: http://awesome-aws-workshops.com/assets/img/awesomebg-extra.png 
ogimagealt: Awesome CDK
---

# Awesome CDK [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome projects related to the [AWS Cloud Development Kit](https://github.com/awslabs/aws-cdk) (AWS CDK).

> DISCLAIMER: this is a personal project and not affiliated with Amazon or AWS.

![last-updated](https://img.shields.io/github/last-commit/eladb/awesome-cdk?color=CB006D&label=last%20updated)
![activity](https://img.shields.io/github/commit-activity/m/eladb/awesome-cdk)


## Contents

- [Construct Libraries](#construct-libraries)
- [Tools](#tools)
- [Training Materials and Sample Code](#training-materials-and-sample-code)
- [Blog Posts & Talks](#blog-posts--talks)
- [Tips & Tricks](#tips--tricks)
- [Related Projects](#related-projects)

## Construct Libraries

This section includes code libraries in various programming languages which vend constructs that can be used in CDK apps.

- [aws-delivlib](https://github.com/awslabs/aws-delivlib): synthesizes CI/CD pipelines for multi-language software delivery (used by the CDK itself)
- [cdk-tweet-queue](https://www.npmjs.com/package/cdk-tweet-queue): fills up an SQS queue with tweets from a tweeter search query.
- [cdk-dynamo-table-viewer](https://www.npmjs.com/package/cdk-dynamo-table-viewer): exposes the contents of an Amazon DynamoDB table through a public HTML page.
- [cdk-tweet-sentiment](https://www.npmjs.com/package/cdk-tweet-sentiment): identify sentiments in tweets and log them into an Amazon DynamoDB table.
- [cdk-watchful](https://github.com/eladb/cdk-watchful): automatic dashboards and alarms for CDK apps
- [Alexa Deployment Pipeline](https://github.com/taimos/cdk-constructs/tree/master/lib/alexa): Construct which creates a CodePipeline to deploy Alexa Skills to Lambda and to the Developer console using AWS SAM and DeployToAlexa action.
- [cdk-codepipeline-slack](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-codepipeline-slack): Cdk component that provisions a #slack approval workflow
- [cdk-github-webhook](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-github-webhook): Cdk component that provisions github webhooks
- [cdk-instanceStopRule](https://github.com/tecracer/cdk-constructs/tree/master/packages/cdk-instanceStopRule) Cdk component which creates an instance with an CloudWatch rule to stop it at the end of the day
- [cdk-static-website](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-static-website): Cdk component that creates a static website using S3, configures CloudFront (CDN) and maps a custom domain via Route53 (DNS)
- [cdk-pull-request-check](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-pull-request-check): Cdk component that automatically check pull requests
- [cdk-passwordless](https://github.com/farminf/aws-cdk-passwordless): construct for having passwordless authentication using userpool
- [cdk-ses-template-mailer](https://github.com/mkrn/cdk-ses-template-mailer): Constructs to create AWS SES email templates + microservice to send templated emails with AWS SES.
- [aws-cdk-pure](https://github.com/fogfish/aws-cdk-pure) - a toolkit to develop purely functional and high-order cloud components with AWS CDK.
- [cdk-iam-generator](https://www.npmjs.com/package/cdk-iam-generator) - Construct to generate IAM Managed Policies and IAM Roles using JSON Configuration
- [cdk-codecommit-backup](https://github.com/cloudcomponents/cdk-components/tree/master/packages/cdk-codecommit-backup) - Backup CodeCommit repositories to S3
- [aws-cdk-dynamodb-seeder](https://github.com/elegantdevelopment/aws-cdk-dynamodb-seeder) - A simple CDK seeder for DynamoDB
- [cdk-sqs-monitored](https://github.com/kamilbiela/cdk-sqs-monitored) - SQS Construct with dead letter queue and configured alarms

## Tools

- [GitHub Action](https://github.com/marketplace/actions/aws-cdk-action) for AWS CDK
- [jsii-publish](https://github.com/udondan/jsii-publish): A [Docker image](https://hub.docker.com/r/udondan/jsii-publish) and [GitHub action](https://github.com/marketplace/actions/jsii-publish) to build and publish CDK constructs created via [JSII](https://github.com/aws/jsii).

## Training Materials and Sample Code

- [Official CDK Examples](https://github.com/aws-samples/aws-cdk-examples)
- [CDK Serverless Workshop](https://cdkworkshop.com/)
- [Infrastructure is Code with the AWS CDK](https://youtu.be/Lh-kVC2r2AU): recording of re:Invent 2018 session
- [GitHub Changelog Crawler](https://github.com/aws-samples/aws-cdk-changelogs-demo) - a fully fledged CDK app written by Nathan Peck which uses Fargate, API Gateway, Lambda, CloudFront, S3, ElastiCache, and Dynamodb.
- [ECS with CI/CD](https://github.com/rix0rrr/cdk-ecs-demo)
- [Example templates for aws cdk](https://github.com/tecracer/cdk-templates): Working TypeScript snippets from several AWS projects
- [Lambda packaging asset](https://gitlab.com/josef.stach/aws-cdk-lambda-asset)
- [Open CDK Guide](https://github.com/kevinslin/open-cdk): Open source guide on CDK and best practices
- [Colorteller Example](https://github.com/denmat/colorteller-aws-cdk): Great example project using Fargate and Appmesh
- [CDK Patterns](https://github.com/cdk-patterns/serverless): An opensource collection of serverless architecture patterns built with CDK
- [Create a CI/CD pipeline using CodePipeline and CodeBuild](https://sbstjn.com/deploy-react-cra-with-cdk-codepipeline-and-codebuild.html): The [cra-pipeline](https://github.com/sbstjn/cra-pipeline) project on GitHub shows an AWS CodePipeline with AWS CodeBuild to deploy a static React application
- [React SPA with server-side rendering on AWS Lambda](https://sbstjn.com/serverless-create-react-app-server-side-rendering-ssr-lamda.html): The [cra-serverless](https://github.com/sbstjn/cra-serverless) project is a serverless architecture to add pre-rendering to a React website created with [create-react-app](https://create-react-app.dev).
- [Mini Tutorial: Setup AWS Lambda + ACM + API Gateway with AWS Cloud Development Kit](https://github.com/shaftoe/api-gateway-lambda-cdk-example): Deploy a functional public API that receives an HTML form (e.g. /contact_us.html) POST request and delivers its data to Pushover notification service.
- [Example of REST API built with CDK](https://github.com/shaftoe/api-l3x-in): Source code that powers REST APIs at https://api.l3x.in/
- [dilbert-feed](https://github.com/mlafeldt/dilbert-feed): A serverless application written in Go that allows you to enjoy Dilbert in your RSS feed reader without any ads.

## Blog Posts & Talks

- [Introduction to how and why CDK](https://www.slideshare.net/ranguard/aws-cdk-introduction-191140240) [keynote/pdf](https://github.com/ranguard/cdk-talk-examples/tree/master/talk)
- [How to Build a CDK Construct Library](https://garbe.io/blog/2019/03/26/construct-your-own-cdk-construct-library/) by Philipp Garbe
- [CDK All The Things: A Whirlwind Tour](https://kevinslin.com/aws/cdk_all_the_things/) by Kevin S Lin
- [Developer Preview Announcement](https://aws.amazon.com/blogs/developer/aws-cdk-developer-preview/)
- [Contributing to the AWS Cloud Development Kit](https://aws.amazon.com/blogs/developer/contributing-to-the-aws-cloud-development-kit/) by Mike Cowgill from Intuit.
- [First look into AWS Cloud Development Kit](https://garbe.io/blog/2018/08/17/first-look-into-cdk/) by Philipp Garbe
- [Boost your AWS Infrastructure with the CDK](https://www.slideshare.net/philippgarbe/boost-your-aws-infrastructure-with-cdk) SlideShare by Philipp Garbe
- [Getting started with AWS CDK for Amazon ECS](https://aws.amazon.com/blogs/compute/getting-started-with-the-aws-cloud-development-kit-for-amazon-ecs/) by Nathan Peck
- [AWS re:Invent 2018, best of show: CDK](https://medium.com/allermedia-techblog/aws-re-invent-2018-best-of-show-cloud-development-kit-cdk-ad1755561ade) (Aller Media Tech Blog)
- [AWS User Group Finland Meetup January 2019](https://youtu.be/IIiIoMGTJec)
- [AWS CDK — a glimpse into the future](https://medium.com/nordcloud-engineering/aws-cdk-a-glimpse-into-the-future-90db660f8a89) (Nordcloud Engineering)
- [AWS Infrastructure as Code with CDK](https://medium.com/avmconsulting-blog/aws-infrastructure-as-code-with-cdk-1d6fa013ce7d) by Ross Rhodes.
- [Callbacks with AWS Step Functions](https://medium.com/swlh/callbacks-with-aws-step-functions-a3dde1bc7203) using CDK by Ross Rhodes.
- [Using the CDK for CodePipelines Setup](https://www.stefreitag.de/wp/2019/03/07/using-aws-cdk-for-code-pipeline-setup/) by Stefan Freitag.
- [Using the CDK for AWS MSK Setup](https://www.stefreitag.de/wp/2019/08/31/paths-are-made-by-walking-or-how-aws-cdk-and-msk-work-together/) by Stefan Freitag.
- [Serverless Dotnet - E01: Intro to AWS CDK](https://www.youtube.com/watch?v=c9UXHPX6-Ns&list=PLbuD6VMxPZScqUXKm2QAc_InCGdP6jKJy) and [Github repository](https://github.com/jakejscott/aws-cdk-phone-verify-api) by Jake Scott.
- [AWS Tech Talk Webinar](https://www.youtube.com/watch?v=ZWCvNFUN-sU)
- [tecRacer Amazon AWS Blog](https://aws-blog.de/tags/cdk.html): Several Blog Posts from aws-blog.de by Gernot Glawe
- [Using CDK to build a UDP NLB Logging Service](https://youtu.be/dXTEVp0ATzo) and [Github Repo](https://github.com/ClouderDex/CDK-UDP-NLB-Demo) by ClouderDex
- [Purely Functional Cloud Components with AWS CDK](https://i.am.fog.fish/2019/08/23/purely-functional-cloud-with-aws-cdk.html)
- [Using the CDK to probe multiple accounts (sfn/lambda/sqs/sechub)](https://fudless.xyz/aws/seedecay/)
- [Scheduled Lambda Functions and CI/CD pipeline with AWS CDK](https://medium.com/hatchsoftware/using-the-aws-cdk-to-build-scheduled-lambda-functions-13eb1674586e) and [Github Repo](https://github.com/HatchSoftware/automatic-aws-db-shutdown-cdk) by Maarten Thoelen
- [AWS Client VPN with mutual TLS](https://lanwen.ru/posts/aws-client-vpn/) by Kirill Merkushev
- [CDK Step Functions](https://dev.to/elthrasher/exploring-aws-cdk-step-functions-1d1e) by Matt Morgan
- [Loading DynamoDB with Custom Resources](https://dev.to/elthrasher/exploring-aws-cdk-loading-dynamodb-with-custom-resources-jlf) by Matt Morgan
- [Loading DynamoDB with Provider Framework](https://dev.to/elthrasher/exploring-aws-cdk-a-million-a-minute-dynamodb-and-providerframework-e92) by Matt Morgan
- [React SPA with server-side rendering on AWS Lambda](https://sbstjn.com/serverless-create-react-app-server-side-rendering-ssr-lamda.html) by Sebastian Müller
- [German: React SPA und server-side rendering (SSR) mit AWS Lambda und CloudFront](https://superluminar.io/2020/02/07/react-spa-und-server-side-rendering-ssr-mit-aws-lambda-cloudfront-und-dem-cdk/) by superluminar GmbH
- [Introducing AWS CDK with a real life Lambda and API gateway example](https://a.l3x.in/2020/02/04/migrating-from-terraform-to-cdk.html) by Alexander Fortin

## Related Projects

- [jsii](https://github.com/awslabs/jsii) - javascript interop interface, the technology that CDK uses to release to multiple programming langauges.
- [punchcard](https://github.com/punchcard/punchcard) - typescript framework to unify infrastructure and runtime code for the CDK, so you can declare constructs and implement runtime logic within the context of one node.js application.
- [cra-template-aws-cdk](https://github.com/luisfarzati/rnbw-aws-cdk/tree/master/packages/cra-template-aws-cdk) Create React App template using AWS CDK for out of the box, simple provisioning of serverless React apps.

## Tips & Tricks

- [Reflect on the CDK Type System](https://gist.github.com/eladb/68a009cf9c953b04a637bac5c40afdbc) (gist)
- [Testing Your Construct Library CodeBuild Configuration Locally](https://github.com/aws/aws-codebuild-docker-images/tree/master/local_builds) with the `jsii/superchain:latest` Docker Image

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.


## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Elad Ben-Israel has waived all copyright and
related or neighboring rights to this work.
