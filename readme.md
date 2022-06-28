# Awesome CDK [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [<img src="https://raw.githubusercontent.com/aws/aws-cdk/master/logo/default-128-dark.png" align="right" alt="CDK">](https://github.com/aws/aws-cdk)

> Curated list of awesome [AWS Cloud Development Kit](https://github.com/awslabs/aws-cdk) (AWS CDK) open-source projects, guides, blogs and other resources.

The AWS Cloud Development Kit (AWS CDK) is an open-source software development framework for defining cloud infrastructure in code.

## Contents

* [Construct Libraries](#construct-libraries)
  * [APIs](#apis)
  * [Databases](#databases)
  * [Static Websites](#static-websites)
  * [Security](#security)
  * [Ops](#ops)
  * [Queue](#queue)
  * [CI/CD](#cicd)
  * [Monitoring](#monitoring)
  * [Workflows](#workflows)
  * [Multi-accounts setup](#multi-accounts-setup)
* [High-Level Frameworks](#high-level-frameworks)
* [Scaffolding](#scaffolding)
* [Language Support](#language-support)
* [Library Publishing](#library-publishing)
* [Tools](#tools)
* [Training Materials and Sample Code](#training-materials-and-sample-code)
* [Blog Posts & Talks](#blog-posts--talks)
* [Related Projects](#related-projects)
* [Tips & Tricks](#tips--tricks)

## Construct Libraries

This section includes code libraries in various programming languages which vend constructs that can be used in CDK apps.

### APIs

* [cdk-chalice](https://github.com/alexpulver/cdk-chalice) - AWS CDK construct for AWS Chalice (Python Serverless Microframework for AWS).
* [auto-cdk](https://github.com/wulfmann/auto-cdk) - Automatically generate api-gateway/lambda integrations with the filesystem (beta).
* [crow-api](https://github.com/thomasstep/crow-api) - Create a serverless API with routes based on your file structure.

### Databases

* [aws-cdk-dynamodb-seeder](https://github.com/elegantdevelopment/aws-cdk-dynamodb-seeder) - A simple CDK seeder for DynamoDB.
* [cdk-tweet-sentiment](https://www.npmjs.com/package/cdk-tweet-sentiment) - Identify sentiments in tweets and log them into an Amazon DynamoDB table.
* [cdk-dynamo-table-viewer](https://github.com/eladb/cdk-dynamo-table-viewer) - Exposes the contents of an Amazon DynamoDB table through a public HTML page.
* [cdk-postgresql](https://github.com/botpress/cdk-postgresql) - AWS CDK Constructs for PostgreSQL.
* [cdk-sqlserver-seeder](https://github.com/kolomied/cdk-sqlserver-seeder) - CDK construct that executes custom SQL scripts against SQL Server database.

### Static Websites

* [cdk-static-website](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-static-website) - CDK component that creates a static website using S3, configures CloudFront (CDN) and maps a custom domain via Route53 (DNS).
* [ness](https://github.com/nessjs/ness) - CDK powered CLI tool for deploying static sites to your AWS account.

### Security

* [cdk-passwordless](https://github.com/farminf/aws-cdk-passwordless) - Construct for having passwordless authentication using userpool.
* [cdk-iam-generator](https://github.com/srihariph/cdk-iam-generator) - Construct to generate IAM Managed Policies and IAM Roles using JSON Configuration.
* [c3](https://github.com/SSHcom/c3) - Enables compliancy with privacy and security best practices.
* [cdk-iam-floyd](https://github.com/udondan/iam-floyd) - IAM policy statement generator with fluent interface.
* [k9-cdk](https://github.com/k9securityio/k9-cdk) - Construct to generate secure S3 bucket policies easily.
* [cdk-cloudfront-authorization](https://github.com/cloudcomponents/cdk-constructs/tree/master/packages/cdk-cloudfront-authorization) - CloudFront with Cognito authentication using Lambda@Edge.
* [aws-firewall-factory](https://github.com/globaldatanet/aws-firewall-factory) - Deploy, update, and stage your WAFs while managing them centrally via FMS.
### Ops

* [cdk-instanceStopRule](https://github.com/tecracer/cdk-constructs/tree/master/packages/cdk-instanceStopRule) - CDK component which creates an instance with a CloudWatch rule to stop it at the end of the day.
* [cdk-time-bomb](https://github.com/jmb12686/cdk-time-bomb) - CDK Construct that implodes your AWS CDK Stack after a set amount of time.

### Queue

* [cdk-tweet-queue](https://www.npmjs.com/package/cdk-tweet-queue) - Fills up an SQS queue with tweets from a tweeter search query.
* [cdk-ses-template-mailer](https://github.com/mkrn/cdk-ses-template-mailer) - Constructs to create AWS SES email templates + microservice to send templated emails with AWS SES.
* [cdk-sqs-monitored](https://github.com/kamilbiela/cdk-sqs-monitored) - SQS Construct with dead letter queue and configured alarms.

### CI/CD

* [aws-delivlib](https://github.com/awslabs/aws-delivlib) - Synthesizes CI/CD pipelines for multi-language software delivery (used by the CDK itself).
* [cdk-blue-green-container-deployment](https://github.com/cloudcomponents/cdk-constructs/tree/master/packages/cdk-blue-green-container-deployment) - Blue/Green container deployment with CodeDeploy.

### Monitoring

* [cdk-watchful](https://github.com/eladb/cdk-watchful) - Automatic dashboards and alarms for CDK apps.
* [aws-cdk-billing-alarm](https://github.com/alvyn279/aws-cdk-billing-alarm) - Construct that sets up email alerts for exceeding an amount on your AWS bill.
* [cdk-monitoring-constructs](https://github.com/cdklabs/cdk-monitoring-constructs) - Use high-level APIs to create monitoring for your AWS apps. Generates dashboards automatically.

### Workflows

* [cdk-pull-request-check](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-pull-request-check) - CDK component that automatically check pull requests.
* [cdk-github-webhook](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-github-webhook) - CDK component that provisions GitHub webhooks.
* [cdk-codepipeline-slack](https://github.com/cloudcomponents/cdk-components/blob/master/packages/cdk-codepipeline-slack) - CDK component that provisions a #slack approval workflow.
* [cdk-codecommit-backup](https://github.com/cloudcomponents/cdk-components/tree/master/packages/cdk-codecommit-backup) - Backup CodeCommit repositories to S3.
* [Alexa Deployment Pipeline](https://github.com/taimos/cdk-constructs/tree/master/lib/alexa) - Construct which creates a CodePipeline to deploy Alexa Skills to Lambda and to the Developer console using AWS SAM and DeployToAlexa action.
* [cdk-developer-tools-notifications](https://github.com/cloudcomponents/cdk-constructs/tree/master/packages/cdk-developer-tools-notifications) - Slack / Microsoft Teams / Email notifications for developer tools: CodeCommit, CodeBuild, CodeDeploy, CodePipeline.
* [aws-pdf-textract-pipeline](https://github.com/aeksco/aws-pdf-textract-pipeline) - ETL pipeline for crawling PDFs from the Web using Puppeteer and transforming their contents into structured data using AWS Textract and storing the results in DynamoDB.

### Multi-accounts setup
* [aws-bootstrap-kit](https://github.com/awslabs/aws-bootstrap-kit) - Creates a multi-account set-up with AWS Organization, AWS SSO, DNS, and AWS CodePipeline.
* [cdk-organizations](https://github.com/pepperize/cdk-organizations) - CDK constructs that helps to provision AWS Organization, Organizational Units (OU), Accounts and Policies.

## High-Level Frameworks

* [punchcard](https://github.com/punchcard/punchcard) - TypeScript framework to unify infrastructure and runtime code for the CDK, so you can declare constructs and implement runtime logic within the context of one Node.js application.
* [aws-cdk-pure](https://github.com/fogfish/aws-cdk-pure) - A toolkit to develop purely functional and high-order cloud components with AWS CDK.
* [cdk-stepfunctions-patterns](https://github.com/kolomied/cdk-stepfunctions-patterns) - A set of Step Functions high-level resiliency patterns.
* [Orkestra](https://github.com/knowsuchagency/orkestra) - An event-driven alternative to Airflow built on the AWS CDK and Step Functions.
* [SST](https://github.com/serverless-stack/serverless-stack) - An open source framework for building serverless applications with CDK. It features a Live Lambda Development environment, to test and debug Lambda functions locally without having to redeploy them.
* [Datajob](https://github.com/vincentclaes/datajob) - Build and deploy a serverless data pipeline or machine learning pipeline on AWS with no effort. 

## Scaffolding

* [ReactJS + Cognito + CDK Starter](https://github.com/vbudilov/reactjs-cognito-starter) - Starter project for ReactJS + Amazon Cognito + Amazon Amplify Framework with AWS CDK support.
* [cra-template-aws-cdk](https://github.com/luisfarzati/rnbw-aws-cdk/tree/master/packages/cra-template-aws-cdk) - Create React App template using AWS CDK for out of the box, simple provisioning of serverless React apps.
* [create-cdk-app](https://github.com/cdk-tools/create-cdk-app) - Create CDK apps from templates.
* [awscdk-jsii-template](https://github.com/pahud/awscdk-jsii-template) - A GitHub template repository to generate a ready environment to build, test and publish your [JSII]((https://github.com/aws/jsii)) construct lib for AWS CDK.

## Language Support

* [AWS-CDK-Kotlin-DSL](https://github.com/justincase-jp/AWS-CDK-Kotlin-DSL) - A Wrapper library of [AWS CDK Java](https://mvnrepository.com/artifact/software.amazon.awscdk). CI automatically generates code and deploys it by daily.
* [aws-cdk-maven-plugin](https://github.com/LinguaRobot/aws-cdk-maven-plugin) - A plugin to define and deploy your AWS CDK applications using Java and Maven.
* [aws-lambda-nodejs-webpack](https://github.com/vvo/aws-lambda-nodejs-webpack) - Alternative Node.js lambda CDK construct, using [webpack](https://webpack.js.org/).
* [aws-lambda-nodejs-esbuild](https://github.com/floydspace/aws-lambda-nodejs-esbuild) - Alternative Node.js lambda CDK construct, using [esbuild](https://github.com/evanw/esbuild).

## Library Publishing

* [GitHub Action](https://github.com/marketplace/actions/aws-cdk-action) - GitHub Action for AWS CDK.
* [jsii-publish](https://github.com/udondan/jsii-publish) - A [Docker image](https://hub.docker.com/r/udondan/jsii-publish) and [GitHub action](https://github.com/marketplace/actions/jsii-publish) to build and publish CDK constructs created via [JSII](https://github.com/aws/jsii).

## Tools

* [CDK-Dia](https://github.com/pistazie/cdk-dia) - Automatic infrastructure diagrams for AWS CDK.

## Training Materials and Sample Code

* [Official CDK Examples](https://github.com/aws-samples/aws-cdk-examples) - A set of example projects for the AWS CDK.
* [CDK Serverless Workshop](https://cdkworkshop.com/) - A workshop that guides you through the process of creating and deploying CDK application.
* [Build an App with AWS Cloud Development Kit course on egghead.io](https://egghead.io/courses/build-an-app-with-the-aws-cloud-development-kit?af=6p5abz)
* [Infrastructure is Code with the AWS CDK](https://youtu.be/Lh-kVC2r2AU) - Recording of re:Invent 2018 session.
* [GitHub Changelog Crawler](https://github.com/aws-samples/aws-cdk-changelogs-demo) - A fully fledged CDK app written by Nathan Peck which uses Fargate, API Gateway, Lambda, CloudFront, S3, ElastiCache, and Dynamodb.
* [ECS with CI/CD](https://github.com/rix0rrr/cdk-ecs-demo) - Demo of deploying ECS application using CDK.
* [Example templates for aws cdk](https://github.com/tecracer/cdk-templates) - Working TypeScript snippets from several AWS projects.
* [Lambda packaging asset](https://gitlab.com/josef.stach/aws-cdk-lambda-asset) - CDK asset which builds lambda function and produces a ZIP file with dependencies.
* [Open CDK Guide](https://github.com/kevinslin/open-cdk) - Open source guide on CDK and best practices.
* [Colorteller Example](https://github.com/denmat/colorteller-aws-cdk) - Great example project using Fargate and Appmesh.
* [CDK Patterns](https://github.com/cdk-patterns/serverless) - An opensource collection of serverless architecture patterns built with CDK.
* [Create a CI/CD pipeline using CodePipeline and CodeBuild](https://sbstjn.com/deploy-react-cra-with-cdk-codepipeline-and-codebuild.html) - The [cra-pipeline](https://github.com/sbstjn/cra-pipeline) project on GitHub shows an AWS CodePipeline with AWS CodeBuild to deploy a static React application.
* [React SPA with server-side rendering on AWS Lambda](https://sbstjn.com/serverless-create-react-app-server-side-rendering-ssr-lamda.html) - The [cra-serverless](https://github.com/sbstjn/cra-serverless) project is a serverless architecture to add pre-rendering to a React website created with [create-react-app](https://create-react-app.dev).
* [Mini Tutorial: Setup AWS Lambda + ACM + API Gateway with AWS Cloud Development Kit](https://github.com/shaftoe/api-gateway-lambda-cdk-example) - Deploy a functional public API that receives an HTML form (e.g. /contact_us.html) POST request and delivers its data to Pushover notification service.
* [Example of REST API built with CDK](https://github.com/shaftoe/api-l3x-in) - Source code that powers REST APIs at https://api.l3x.in/.
* [dilbert-feed](https://github.com/mlafeldt/dilbert-feed) - A serverless application written in Go that allows you to enjoy Dilbert in your RSS feed reader without any ads.
* [django-postgres-vue-gitlab-ecs](https://gitlab.com/verbose-equals-true/django-postgres-vue-gitlab-ecs) - An example Django + Vue.js web app deployed with CDK using GitLab CI.
* [nextjs-vercel-aws-cdk-example](https://github.com/vvo/nextjs-vercel-aws-cdk-example) - A PostgreSQL (RDS), EventBridge (crons) and SNS (background jobs) example along with a Next.js application.
* [Create and Publish CDK Constructs Using projen and jsii](https://github.com/seeebiii/projen-test) - A step-by-step guide with sample code to create a new CDK construct using [projen](https://github.com/projen/projen) and `jsii` and publish it to npm, Maven Central, PyPi and NuGet.

## Blog Posts & Talks

* [Introduction to how and why CDK](https://www.slideshare.net/ranguard/aws-cdk-introduction-191140240) - By Leo Lapworth.
* [How to Build a CDK Construct Library](https://garbe.io/blog/2019/03/26/construct-your-own-cdk-construct-library/) - By Philipp Garbe.
* [CDK All The Things: A Whirlwind Tour](https://kevinslin.com/aws/cdk_all_the_things/) - By Kevin S Lin.
* [AWS CDK Developer Preview Announcement](https://aws.amazon.com/blogs/developer/aws-cdk-developer-preview/) - The first AWS CDK Developer Preview announced on on 27 August 2018.
* [Contributing to the AWS Cloud Development Kit](https://aws.amazon.com/blogs/developer/contributing-to-the-aws-cloud-development-kit/) - By Mike Cowgill from Intuit.
* [First look into AWS Cloud Development Kit](https://garbe.io/blog/2018/08/17/first-look-into-cdk/) - By Philipp Garbe.
* [Boost your AWS Infrastructure with the CDK](https://www.slideshare.net/philippgarbe/boost-your-aws-infrastructure-with-cdk) - SlideShare by Philipp Garbe.
* [Getting started with AWS CDK for Amazon ECS](https://aws.amazon.com/blogs/compute/getting-started-with-the-aws-cloud-development-kit-for-amazon-ecs/) - By Nathan Peck.
* [AWS re:Invent 2018, best of show: CDK](https://medium.com/allermedia-techblog/aws-re-invent-2018-best-of-show-cloud-development-kit-cdk-ad1755561ade) - Aller Media Tech Blog.
* [AWS Cloud Development Kit introduction with Live Demos](https://youtu.be/IIiIoMGTJec) - AWS User Group Finland Meetup January 2019.
* [AWS CDK — a glimpse into the future](https://medium.com/nordcloud-engineering/aws-cdk-a-glimpse-into-the-future-90db660f8a89) - By Nordcloud Engineering.
* [AWS Infrastructure as Code with CDK](https://medium.com/avmconsulting-blog/aws-infrastructure-as-code-with-cdk-1d6fa013ce7d) - By Ross Rhodes.
* [Callbacks with AWS Step Functions](https://medium.com/swlh/callbacks-with-aws-step-functions-a3dde1bc7203) - By Ross Rhodes.
* [Using the CDK for CodePipelines Setup](https://www.stefreitag.de/wp/2019/03/07/using-aws-cdk-for-code-pipeline-setup/) - By Stefan Freitag.
* [Using the CDK for AWS MSK Setup](https://www.stefreitag.de/wp/2019/08/31/paths-are-made-by-walking-or-how-aws-cdk-and-msk-work-together/) - By Stefan Freitag.
* [Serverless Dotnet - E01: Intro to AWS CDK](https://youtu.be/c9UXHPX6-Ns) - By Jake Scott.
* [GitHub repository](https://github.com/jakejscott/aws-cdk-phone-verify-api) - By Jake Scott.
* [Infrastructure is Code with the AWS CDK](https://youtu.be/ZWCvNFUN-sU) - AWS Tech Talk Webinar.
* [tecRacer Amazon AWS Blog](https://aws-blog.de/tags/cdk.html) - Several Blog Posts from aws-blog.de by Gernot Glawe.
* [Using CDK to build a UDP NLB Logging Service](https://youtu.be/dXTEVp0ATzo) - By ClouderDex.
* [GitHub Repo](https://github.com/ClouderDex/CDK-UDP-NLB-Demo) - By ClouderDex.
* [Purely Functional Cloud Components with AWS CDK](https://i.am.fog.fish/2019/08/23/purely-functional-cloud-with-aws-cdk.html) - Bu fogfish.
* [Using the CDK to probe multiple accounts (sfn/lambda/sqs/sechub)](https://fudless.xyz/aws/seedecay/) - Blog post from [fudless.xyz](https://fudless.xyz).
* [Scheduled Lambda Functions and CI/CD pipeline with AWS CDK](https://medium.com/hatchsoftware/using-the-aws-cdk-to-build-scheduled-lambda-functions-13eb1674586e) - By Maarten Thoelen.
* [GitHub Repo](https://github.com/HatchSoftware/automatic-aws-db-shutdown-cdk) - By Maarten Thoelen.
* [AWS Client VPN with mutual TLS](https://lanwen.ru/posts/aws-client-vpn/) - By Kirill Merkushev.
* [CDK Step Functions](https://dev.to/elthrasher/exploring-aws-cdk-step-functions-1d1e) - By Matt Morgan.
* [Loading DynamoDB with Custom Resources](https://dev.to/elthrasher/exploring-aws-cdk-loading-dynamodb-with-custom-resources-jlf) - By Matt Morgan.
* [Loading DynamoDB with Provider Framework](https://dev.to/elthrasher/exploring-aws-cdk-a-million-a-minute-dynamodb-and-providerframework-e92) - By Matt Morgan.
* [German: React SPA und server-side rendering (SSR) mit AWS Lambda und CloudFront](https://superluminar.io/2020/02/07/react-spa-und-server-side-rendering-ssr-mit-aws-lambda-cloudfront-und-dem-cdk/) - By superluminar GmbH.
* [Introducing AWS CDK with a real life Lambda and API gateway example](https://a.l3x.in/2020/02/04/migrating-from-terraform-to-cdk.html) - By Alexander Fortin.
* [CloudWatch Dashboards as Code (the Right Way) Using AWS CDK](https://medium.com/poka-techblog/cloudwatch-dashboards-as-code-the-right-way-using-aws-cdk-1453309c5481) - By Simon-Pierre Gingras.
* [Coding the Jamstack missing parts: databases, crons & background jobs](https://dev.to/vvo/coding-the-jamstack-missing-parts-databases-crons-background-jobs-1bpj) - By Vincent Voyer.
* [AWS CDK Continuous Integration and Delivery Using Travis CI](https://medium.com/better-programming/aws-cdk-continuous-integration-and-delivery-using-travis-ci-ee5dd7549434) - By Thomas Poignant.
* [Custom Resources with AWS CDK](https://medium.com/cyberark-engineering/custom-resources-with-aws-cdk-d9a8fad6b673?source=friends_link&sk=549fcf9d998bbea304bdd8d834aca9e6) - By Roy Ben-Yosef.
* [Recommended AWS CDK project structure for Python applications](https://aws.amazon.com/blogs/developer/recommended-aws-cdk-project-structure-for-python-applications/) - By Alex Pulver.

## Related Projects

* [jsii](https://github.com/awslabs/jsii) - JavaScript interop interface, the technology that CDK uses to create language bindings (currently supports .NET, Java and Python).
* [cdk8s](https://github.com/awslabs/cdk8s/) - Define Kubernetes native apps and abstractions using object-oriented programming.
* [cdktf](https://github.com/hashicorp/terraform-cdk) - Define infrastructure resources using programming constructs and provision them using HashiCorp Terraform.
* [cdktg](https://github.com/hupe1980/cdk-threagile) - Agile Threat Modeling as Code.

## Tips & Tricks

* [Reflect on the CDK Type System](https://gist.github.com/eladb/68a009cf9c953b04a637bac5c40afdbc) - Explore the CDK's type system.
* [Testing Your Construct Library CodeBuild Configuration Locally](https://github.com/aws/aws-codebuild-docker-images/tree/master/local_builds) - With the `jsii/superchain:latest` Docker Image.

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.
