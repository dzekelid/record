---
name: AWS Kinesis
x-slug: aws-kinesis
description: Amazon Kinesis Firehose is the easiest way to load streaming data into
  AWS. It can capture, transform, and load streaming data into Amazon Kinesis Analytics,
  Amazon S3, Amazon Redshift, and Amazon Elasticsearch Service, enabling near real-time
  analytics with existing business intelligence tools and dashboards you are already
  using today.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonKinesis_AmazonKinesisFirehose.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Record
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-kinesis/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Kinesis Firehose API - Put Record
  x-api-slug: actionputrecord-get
  description: writes a single data record into an Amazon Kinesis Firehose delivery
    stream.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonKinesis_AmazonKinesisFirehose.png
  humanURL: https://aws.amazon.com/kinesis/
  baseURL: :///
  tags: Amazon Web Services, Real Time, Data, Stack Network, Streaming, API Service
    Provider, API Service Provider, API Provider, SDIO Competition, Databases, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-kinesis/actionputrecord-get-openapi.md
- name: AWS Kinesis Firehose API - Put Record Batch
  x-api-slug: actionputrecordbatch-get
  description: |-
    writes multiple data records into a delivery stream in a single call, which can
             achieve higher throughput per producer than when writing single records.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AmazonKinesis_AmazonKinesisFirehose.png
  humanURL: https://aws.amazon.com/kinesis/
  baseURL: :///
  tags: Amazon Web Services, Real Time, Data, Stack Network, Streaming, API Service
    Provider, API Service Provider, API Provider, SDIO Competition, Databases, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-kinesis/actionputrecordbatch-get-openapi.md
x-common:
- type: x-hacker-news-search
  url: Amazon Kinesis
- type: x-api-gallery
  url: http://aws.key.management.service.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.kinesis.stack.network
- type: x-console
  url: https://console.aws.amazon.com/firehose/
- type: x-documentation
  url: http://docs.aws.amazon.com/firehose/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/kinesis/firehose/faqs/
- type: x-getting-started
  url: https://aws.amazon.com/kinesis/firehose/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/kinesis/firehose/pricing/
- type: x-website
  url: https://aws.amazon.com/kinesis/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---