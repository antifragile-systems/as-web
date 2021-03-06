# :hatching_chick: Antifragile Systems :earth_africa: website

[![Build Status](https://travis-ci.org/antifragile-systems/antifragile.systems.svg?branch=master)](https://travis-ci.org/antifragile-systems/antifragile.systems)
[![Coverage Status](https://coveralls.io/repos/github/antifragile-systems/antifragile.systems/badge.svg?branch=master)](https://coveralls.io/github/antifragile-systems/antifragile.systems?branch=master)
[![](https://img.shields.io/github/release/antifragile-systems/antifragile.systems.svg)](https://github.com/antifragile-systems/antifragile.systems/releases)

> Antifragile Systems website

<p align="center"><img src="share/github/overview.png" width="720"></p>

### Features
* Host files on a [AWS S3](https://aws.amazon.com/s3) bucket and deliver them :globe_with_meridians: worldwide through [AWS CloudFront](https://aws.amazon.com/cloudfront) :white_check_mark:

### How to develop
Clone the GitHub repo
```
git clone https://github.com/antifragile-systems/antifragile.systems.git
```

Change current directory
```
cd antifragile.systems
```

Run the NPM script that will deploy
```
npm run start
```

#### Available environment variables
Variable | Description | Required | Default value
:---:|:---:|:---:|:---:
WEBPACK_DEV_PORT | The port be used by the Webpack development server. | false | `3000`
ENVIRONMENT | The environment the app is running on. | false | `production`

### How to deploy
Clone the GitHub repo
```
git clone https://github.com/antifragile-systems/antifragile.systems.git
```

Change current directory
```
cd antifragile.systems
```

Run the NPM script that will deploy
```
npm run deploy
```

#### Available environment variables
Variable | Description | Required | Default value
:---:|:---:|:---:|:---:
AWS_REGION | AWS region used for S3 and CloudFront. | true | `undefined`
AWS_ACCESS_KEY_ID | AWS access key used for S3 and CloudFront. | true | `undefined`
AWS_SECRET_ACCESS_KEY | AWS secret access key used for S3 and CloudFront. | true | `undefined`
AWS_S3_BUCKET | The bucket to host the website files. | false | `antifragile.systems`
AWS_CLOUDFRONT_DISTRIBUTION_ID | The distribution ID to invalidate its cache. | true | `undefined`
ENVIRONMENT | The environment the app is running on. | false | `production`
