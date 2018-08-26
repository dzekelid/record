---
name: BetterDoctor
x-slug: betterdoctor
description: BetterDoctor helps people find and connect to the best doctors through
  our consumer app, doctor marketing services, and API. Our mission is to help increase
  transparency in healthcare and help consumers make better decisions.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
x-kinRank: "8"
x-alexaRank: "625342"
tags: Record
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/apis.md
specificationVersion: "0.14"
apis:
- name: BetterDoctor - Record search
  x-api-slug: validations-get
  description: 'The endpoint can be used to identify providers with validation data.
    The search supports BetterDoctor unique provider identifier, National Provider
    Identifier (NPI) or reference uid based provider lookups. BetterDoctor identifiers
    and NPIs for doctors and practices can be discovered using BetterDoctor API???s
    search functionalities. <br><h4 style=''margin-bottom: 0px !important;''> Return
    Headers </h4> <div>Last-Modified: Timestamp of the last validation made over the
    matching validations. The value can be used to query changes in the validation
    status for the provider using since parameter in collaboration with HEAD method.</div>'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01
  tags: Healthcare, Doctors, Technology, SaaS, Mobile, Insurance, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validations-get-openapi.md
- name: BetterDoctor - Check if new records exists
  x-api-slug: validations-head
  description: 'The endpoint can be used to identify providers with validation data,
    and discover changes. It providers search functionalities like its GET method
    alternative, but does not return any validation data. Instead of the data itself,
    it returns 200 OK if matching validation documents based on the given query are
    found. And it returns 304 if no validation documents are found after the timestamp
    given using If-Modified-Since HTTP header or since parameter. <br><h4 style=''margin-bottom:
    0px !important;''> Return Headers </h4> <div>Last-Modified: Timestamp of the last
    validation made over the matching validations. </div>'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01
  tags: Healthcare, Doctors, Technology, SaaS, Mobile, Insurance, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validations-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validations-head-openapi.md
- name: BetterDoctor - Retrieve a specific record
  x-api-slug: validationsuid-get
  description: 'Returns requested validation document. The endpoint is a conveniece
    method to check status and accepted data of a specific validation, like after
    creation of a validation. The response consist of raw data from the validation
    event and related validation information. <br><h4 style=''margin-bottom: 0px !important;''>
    Return Headers </h4> <div>Last-Modified: Timestamp of the validation made.</div>'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01
  tags: Healthcare, Doctors, Technology, SaaS, Mobile, Insurance, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validationsuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validationsuid-get-openapi.md
- name: BetterDoctor - Check if a specific record exists
  x-api-slug: validationsuid-head
  description: 'The endpoint can be used to discover if a validation document exists
    in the API. <br><h4 style=''margin-bottom: 0px !important;''> Return Headers </h4>
    <div>Last-Modified: Timestamp of the validation made.</div>'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18991-betterdoctor.jpg
  humanURL: https://developer.betterdoctor.com
  baseURL: https://api.betterdoctor.com//2016-03-01
  tags: Healthcare, Doctors, Technology, SaaS, Mobile, Insurance, API Provider, Profiles,
    General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validationsuid-head-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/record/master/_listings/betterdoctor/validationsuid-head-openapi.md
x-common:
- type: x-api-gallery
  url: http://bc.route.planner.api.gallery.streamdata.io
- type: x-api-stack
  url: http://betterdoctor.stack.network
- type: x-blog
  url: https://betterdoctor.com/health/
- type: x-blog-rss
  url: https://betterdoctor.com/health/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/betterdoctor-inc
- type: x-developer
  url: https://developer.betterdoctor.com
- type: x-email
  url: hello@betterdoctor.com
- type: x-email
  url: press@betterdoctor.com
- type: x-email
  url: tony@betterdoctor.com
- type: x-email
  url: privacy@betterdoctor.com
- type: x-email
  url: support@betterdoctor.com
- type: x-email
  url: copyright@betterdoctor.com
- type: x-github
  url: https://github.com/betterdoctor
- type: x-twitter
  url: https://twitter.com/betterdoctor
- type: x-website
  url: https://betterdoctor.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---