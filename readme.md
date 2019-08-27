# Awesome CDK [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome projects related to the [AWS Cloud Development Kit](https://github.com/awslabs/aws-cdk) (AWS CDK).

> DISCLAIMER: this is a personal project and not affiliated with Amazon or AWS.

## Contents

- [Construct Libraries](#construct-libraries)
- [Tools](#tools)
- [Training Materials and Sample Code](#training-materials-and-sample-code)
- [Blog Posts](#blog-posts)
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
- [cdk-static-website](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-static-website): Cdk component that creates a static website using S3, configures CloudFront (CDN) and maps a custom domain via Route53 (DNS)
- [cdk-pull-request-check](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-pull-request-check): Cdk component that automatically check pull requests
- [cdk-passwordless](https://github.com/farminf/aws-cdk-passwordless): construct for having passwordless authentication using userpool

## Tools

- [GitHub Action](https://github.com/marketplace/actions/aws-cdk-action) for AWS CDK

## Training Materials and Sample Code

- [Official CDK Examples](https://github.com/aws-samples/aws-cdk-examples)
- [CDK Serverless Workshop](https://cdkworkshop.com/)
- [Infrastructure is Code with the AWS CDK](https://youtu.be/Lh-kVC2r2AU): recording of re:Invent 2018 session
- [GitHub Changelog Crawler](https://github.com/aws-samples/aws-cdk-changelogs-demo) - a fully fledged CDK app written by Nathan Peck which uses Fargate, API Gateway, Lambda, CloudFront, S3, ElastiCache, and Dynamodb.
- [ECS with CI/CD](https://github.com/rix0rrr/cdk-ecs-demo)

## Blog Posts & Talks

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
- [AWS Infrastructure as Code with CDK](https://itnext.io/aws-infrastructure-as-code-with-cdk-1d6fa013ce7d) by Ross Rhodes.
- [Using the CDK for CodePipelines Setup](https://www.stefreitag.de/wp/2019/03/07/using-aws-cdk-for-code-pipeline-setup/) at Th!nk Pos!t!ve.
- [Serverless Dotnet - E01: Intro to AWS CDK](https://www.youtube.com/watch?v=c9UXHPX6-Ns&list=PLbuD6VMxPZScqUXKm2QAc_InCGdP6jKJy) and [Github repository](https://github.com/jakejscott/aws-cdk-phone-verify-api) by Jake Scott.

## Related Projects

- [jsii](https://github.com/awslabs/jsii) - javascript interop interface, the technology the CDK uses to release to multiple programming langauges.

## Tips & Tricks

- [Reflect on the CDK Type System](https://gist.github.com/eladb/68a009cf9c953b04a637bac5c40afdbc) (gist)
- [Testing Your Construct Library CodeBuild Configuration Locally](https://github.com/aws/aws-codebuild-docker-images/tree/master/local_builds) with the `jsii/superchain:latest` Docker Image

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.


## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Elad Ben-Israel has waived all copyright and
related or neighboring rights to this work.
