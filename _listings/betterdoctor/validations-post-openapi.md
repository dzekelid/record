---
swagger: "2.0"
x-collection-name: BetterDoctor
x-complete: 0
info:
  title: BetterDoctor Add a new record
  description: 'Creates validation document using the request body, and returns the
    document created with unique identifier in Location header for reference. This
    is how validation data is submitted to BetterDoctor for addition to the API. The
    posted document must conform to BetterDoctor???s JSON schema for validation objects,
    see included model specification for more information. <br><h4 style=''margin-bottom:
    0px !important;''> Return Headers </h4> <div>Location: The uid of the created
    document. This can be used to access the document again without executing a search.</div>'
  version: 1.0.0
host: api.betterdoctor.com
basePath: /2016-03-01
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /validations:
    post:
      summary: Add a new record
      description: 'Creates validation document using the request body, and returns
        the document created with unique identifier in Location header for reference.
        This is how validation data is submitted to BetterDoctor for addition to the
        API. The posted document must conform to BetterDoctor???s JSON schema for
        validation objects, see included model specification for more information.
        <br><h4 style=''margin-bottom: 0px !important;''> Return Headers </h4> <div>Location:
        The uid of the created document. This can be used to access the document again
        without executing a search.</div>'
      operationId: creates-validation-document-using-the-request-body-and-returns-the-document-created-with-unique-iden
      x-api-path-slug: validations-post
      parameters:
      - in: query
        name: user_key
        description: Your API access key
      - in: body
        name: validation
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---