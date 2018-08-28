---
name: AWS Config
x-slug: aws-config
description: AWS Config is a fully managed service that provides you with an AWS resource
  inventory, configuration history, and configuration change notifications to enable
  security and governance. Config Rules enables you to create rules that automatically
  check the configuration of AWS resources recorded by AWS Config.With AWS Config,
  you can discover existing and deleted AWS resources, determine your overall compliance
  against rules, and dive into configuration details of a resource at any point in
  time. These capabilities enable compliance auditing, security analysis, resource
  change tracking, and troubleshooting.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Record
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-config/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Config API - Delete Configuration Recorder
  x-api-slug: actiondeleteconfigurationrecorder-get
  description: Deletes the configuration recorder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: :///
  tags: Amazon Web Services, Applications, Regulations, Governance, Security, Authentication,
    Stack Network, API Service Provider, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-config/actiondeleteconfigurationrecorder-get-openapi.md
- name: AWS Config API - Describe Configuration Recorders
  x-api-slug: actiondescribeconfigurationrecorders-get
  description: Returns the details for the specified configuration recorders.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: :///
  tags: Amazon Web Services, Applications, Regulations, Governance, Security, Authentication,
    Stack Network, API Service Provider, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-config/actiondescribeconfigurationrecorders-get-openapi.md
- name: AWS Config API - Describe Configuration Recorder Status
  x-api-slug: actiondescribeconfigurationrecorderstatus-get
  description: Returns the current status of the specified configuration recorder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: :///
  tags: Amazon Web Services, Applications, Regulations, Governance, Security, Authentication,
    Stack Network, API Service Provider, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-config/actiondescribeconfigurationrecorderstatus-get-openapi.md
- name: AWS Config API - Put Configuration Recorder
  x-api-slug: actionputconfigurationrecorder-get
  description: Creates a new configuration recorder to record the selected resource
    configurations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: :///
  tags: Amazon Web Services, Applications, Regulations, Governance, Security, Authentication,
    Stack Network, API Service Provider, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-config/actionputconfigurationrecorder-get-openapi.md
- name: AWS Config API - Start Configuration Recorder
  x-api-slug: actionstartconfigurationrecorder-get
  description: Starts recording configurations of the AWS resources you have selected
    to record in your AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: :///
  tags: Amazon Web Services, Applications, Regulations, Governance, Security, Authentication,
    Stack Network, API Service Provider, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-config/actionstartconfigurationrecorder-get-openapi.md
- name: AWS Config API - Stop Configuration Recorder
  x-api-slug: actionstopconfigurationrecorder-get
  description: Stops recording configurations of the AWS resources you have selected
    to record in your AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Management-Tools_AWSConfig.png
  humanURL: https://aws.amazon.com/config/
  baseURL: :///
  tags: Amazon Web Services, Applications, Regulations, Governance, Security, Authentication,
    Stack Network, API Service Provider, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/aws-config/actionstopconfigurationrecorder-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.cognito.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.config.stack.network
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/configservice/index.html
- type: x-console
  url: https://console.aws.amazon.com/config
- type: x-documentation
  url: http://docs.aws.amazon.com/config/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/config/faq/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=184
- type: x-getting-started
  url: https://aws.amazon.com/config/getting-started/
- type: x-partners
  url: https://aws.amazon.com/config/partners/
- type: x-pricing
  url: https://aws.amazon.com/config/pricing/
- type: x-support
  url: https://console.aws.amazon.com/support/
- type: x-website
  url: https://aws.amazon.com/config/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---