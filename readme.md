# Awesome CDK [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of awesome projects related to the [AWS Cloud Development Kit](https://github.com/awslabs/aws-cdk) (AWS CDK).

> DISCLAIMER: this is a personal project and not affiliated with Amazon or AWS.

## Contents

- [Construct Libraries](#construct-libraries)
- [Training Materials](#training-materials)
- [Blog Posts](#blog-posts)
- [Tips & Tricks](#tips--tricks)
- [Released Projects](#related-projects)

## Construct Libraries

This section includes code libraries in various programming languages which vend constructs that can be used in CDK apps.

- [aws-delivlib](https://github.com/awslabs/aws-delivlib): synthesizes CI/CD pipelines for multi-language software delivery (used by the CDK itself)
- [cdk-tweet-queue](https://www.npmjs.com/package/cdk-tweet-queue): fills up an SQS queue with tweets from a tweeter search query.
- [cdk-dynamo-table-viewer](https://www.npmjs.com/package/cdk-dynamo-table-viewer): exposes the contents of an Amazon DynamoDB table through a public HTML page.
- [cdk-tweet-sentiment](https://www.npmjs.com/package/cdk-tweet-sentiment): identify sentiments in tweets and log them into an Amazon DynamoDB table.

## Training Materials and Sample Code

- [Official CDK Examples](https://github.com/aws-samples/aws-cdk-examples)
- [CDK Serverless Workshop](https://cdkworkshop.com/)
- [Infrastructure is Code with the AWS CDK](https://youtu.be/Lh-kVC2r2AU): recording of re:Invent 2018 session

## Blog Posts & Talks

- [Developer Preview Announcement](https://aws.amazon.com/blogs/developer/aws-cdk-developer-preview/)
- [Contributing to the AWS Cloud Development Kit](https://aws.amazon.com/blogs/developer/contributing-to-the-aws-cloud-development-kit/) by Mike Cowgill from Intuit.
- [First look into AWS Cloud Development Kit](https://garbe.io/blog/2018/08/17/first-look-into-cdk/) by Philipp Garbe
- [Getting started with AWS CDK for Amazon ECS](https://aws.amazon.com/blogs/compute/getting-started-with-the-aws-cloud-development-kit-for-amazon-ecs/) by Nathan Peck
- [AWS re:Invent 2018, best of show: CDK](https://medium.com/allermedia-techblog/aws-re-invent-2018-best-of-show-cloud-development-kit-cdk-ad1755561ade) (Aller Media Tech Blog)
- [AWS User Group Finland Meetup January 2019](https://youtu.be/IIiIoMGTJec)
- [AWS CDK — a glimpse into the future](https://medium.com/nordcloud-engineering/aws-cdk-a-glimpse-into-the-future-90db660f8a89) (Nordcloud Engineering)

## Related Projects

- [jsii](https://github.com/awslabs/jsii) - javascript interop interface, the technology the CDK uses to release to multiple programming langauges.

## Tips & Tricks

- [Reflect on the CDK Type System](https://gist.github.com/eladb/68a009cf9c953b04a637bac5c40afdbc) (gist)

## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.


## License

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Elad Ben-Israel has waived all copyright and
related or neighboring rights to this work.
