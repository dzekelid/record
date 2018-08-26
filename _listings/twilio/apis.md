---
name: Twilio
x-slug: twilio
description: Cloud communications platform for building SMS, Voice & Messaging applications
  on an API built for global scale. Get started with a free trial.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
x-kinRank: "10"
x-alexaRank: "9195"
tags: Record
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/apis.md
specificationVersion: "0.14"
apis:
- name: Twilio - Get Recordings
  x-api-slug: accountsaccountsidcallscallsidrecordings-format-get
  description: Returns a list of Recording resource representations, each representing
    anrecording generated during the course of a phone call.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Voice, SMS, Voice, MMS API, MMS, API LIfeyclessss, Getting Started Example,
    Service Level Agreement, Stack Network, Stack, Technology, SaaS, Telecommunications,
    Enterprise, internet, SMS, Telecommunications, Messages, Messages, Relative Data,
    Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidcallscallsidrecordings-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidcallscallsidrecordings-format-get-openapi.md
- name: Twilio - Get Recordings
  x-api-slug: accountsaccountsidrecordings-get
  description: Returns a list of Recording resource representations, each representing
    anrecording generated during the course of a phone call.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Voice, SMS, Voice, MMS API, MMS, API LIfeyclessss, Getting Started Example,
    Service Level Agreement, Stack Network, Stack, Technology, SaaS, Telecommunications,
    Enterprise, internet, SMS, Telecommunications, Messages, Messages, Relative Data,
    Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordings-get-openapi.md
- name: Twilio - Delete Recording
  x-api-slug: accountsaccountsidrecordingsrecordingsid-delete
  description: Deletes a recording  from your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Voice, SMS, Voice, MMS API, MMS, API LIfeyclessss, Getting Started Example,
    Service Level Agreement, Stack Network, Stack, Technology, SaaS, Telecommunications,
    Enterprise, internet, SMS, Telecommunications, Messages, Messages, Relative Data,
    Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordingsrecordingsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordingsrecordingsid-delete-openapi.md
- name: Twilio - Get Recording
  x-api-slug: accountsaccountsidrecordingsrecordingsid-get
  description: Returns one of several representations:nWithout an extension, or with
    a .wav, a binary WAV audio file is returnednwith mime-type audio/x-wav.nAppending
    .mp3 to the URI returns a binary MP3 audio file with mime-typentype audio/mpeg.nAppending
    .xml to the URI returns a XML representation.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Voice, SMS, Voice, MMS API, MMS, API LIfeyclessss, Getting Started Example,
    Service Level Agreement, Stack Network, Stack, Technology, SaaS, Telecommunications,
    Enterprise, internet, SMS, Telecommunications, Messages, Messages, Relative Data,
    Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordingsrecordingsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordingsrecordingsid-get-openapi.md
- name: Twilio - Get Recording Transcriptions
  x-api-slug: accountsaccountsidrecordingsrecordingsidtranscriptions-get
  description: Returns a set of Transcription resource representations that includes
    pagingninformation.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Voice, SMS, Voice, MMS API, MMS, API LIfeyclessss, Getting Started Example,
    Service Level Agreement, Stack Network, Stack, Technology, SaaS, Telecommunications,
    Enterprise, internet, SMS, Telecommunications, Messages, Messages, Relative Data,
    Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordingsrecordingsidtranscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidrecordingsrecordingsidtranscriptions-get-openapi.md
- name: Twilio - Get Account Usage Record
  x-api-slug: accountsaccountsidusagerecords-get
  description: Returns UsageRecords for all usage categories. The list includes pagingninformation.nBy
    default, the UsageRecords resource will return one UsageRecord forneach Category,
    representing all usage accrued all-time for the account.nYou can filter the usage
    Category or change the date-range over which usagenis counted using optional GET
    query parameters.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Voice, SMS, Voice, MMS API, MMS, API LIfeyclessss, Getting Started Example,
    Service Level Agreement, Stack Network, Stack, Technology, SaaS, Telecommunications,
    Enterprise, internet, SMS, Telecommunications, Messages, Messages, Relative Data,
    Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidusagerecords-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidusagerecords-get-openapi.md
- name: Twilio - Get Account Usage Record Sub Resource
  x-api-slug: accountsaccountsidusagerecordssubresource-get
  description: Returns UsageRecords for all usage categories for a specified period.n
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/143-twilio.jpg
  humanURL: http://www.twilio.com
  baseURL: https://api.twilio.com//2010-04-01/
  tags: Voice, SMS, Voice, MMS API, MMS, API LIfeyclessss, Getting Started Example,
    Service Level Agreement, Stack Network, Stack, Technology, SaaS, Telecommunications,
    Enterprise, internet, SMS, Telecommunications, Messages, Messages, Relative Data,
    Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidusagerecordssubresource-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/twilio/accountsaccountsidusagerecordssubresource-get-openapi.md
x-common:
- type: x--net-library
  url: https://www.twilio.com/docs/csharp/install
- type: x-acceptable-use-policy
  url: https://www.twilio.com/legal/aup
- type: x-api-gallery
  url: http://tvmaze.api.gallery.streamdata.io
- type: x-api-stack
  url: http://twilio.stack.network
- type: x-application-gallery
  url: https://www.twilio.com/showcase
- type: x-base-url
  url: https://api.twilio.com
- type: x-blog
  url: http://www.twilio.com/blog
- type: x-blog-rss
  url: http://www.twilio.com/blog/feed
- type: x-community-supported-libraries
  url: https://www.twilio.com/docs/libraries
- type: x-contact-form
  url: https://www.twilio.com/help/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/twilio
- type: x-crunchbase
  url: https://crunchbase.com/organization/twilio
- type: x-documentation
  url: https://www.twilio.com/docs/api
- type: x-email
  url: help@twilio.com
- type: x-email
  url: privacy@twilio.com
- type: x-email
  url: legalnotices@twilio.com
- type: x-email
  url: trademark@twilio.com
- type: x-email
  url: kyleky@twilio.com
- type: x-getting-started
  url: https://www.twilio.com/docs/quickstart
- type: x-github
  url: https://github.com/twilio
- type: x-how-to-guides
  url: https://www.twilio.com/docs/howto
- type: x-java-library
  url: https://www.twilio.com/docs/java/install
- type: x-node-js-library
  url: https://www.twilio.com/docs/node/install
- type: x-paid-support
  url: https://www.twilio.com/premium-support#features
- type: x-partners
  url: https://www.twilio.com/partners
- type: x-php-library
  url: https://www.twilio.com/docs/php/install
- type: x-pricing
  url: https://www.twilio.com/pricing
- type: x-privacy
  url: https://www.twilio.com/legal/privacy
- type: x-python-library
  url: https://www.twilio.com/docs/python/install
- type: x-ruby-library
  url: https://www.twilio.com/docs/ruby/install
- type: x-salesforce-pdk
  url: https://www.twilio.com/docs/salesforce/install
- type: x-security
  url: https://www.twilio.com/docs/security
- type: x-service-level-agreement
  url: https://www.twilio.com/legal/service-level-agreement
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/twilio
- type: x-status
  url: http://status.twilio.com/
- type: x-status-rss
  url: http://status.twilio.com/rss
- type: x-terms-of-service
  url: https://www.twilio.com/legal/tos
- type: x-trademarks
  url: https://www.twilio.com/legal/trademark
- type: x-transparency-report
  url: https://www.twilio.com/blog/2015/07/transparency-report-for-government-requests-for-customer-information.html
- type: x-transparency-report
  url: https://www.twilio.com/legal/transparency
- type: x-twitter
  url: https://twitter.com/twilio
- type: x-website
  url: http://www.twilio.com
- type: x-website
  url: http://twilio.com
- type: x-website
  url: http://stackoverflow.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---