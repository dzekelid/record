---
swagger: "2.0"
x-collection-name: BetterDoctor
x-complete: 1
info:
  title: BetterDoctor
  description: betterdoctor-helps-people-find-and-connect-to-the-best-doctors-through-our-consumer-app-doctor-marketing-services-and-api--our-mission-is-to-help-increase-transparency-in-healthcare-and-help-consumers-make-better-decisions-
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
    get:
      summary: Record search
      description: 'The endpoint can be used to identify providers with validation
        data. The search supports BetterDoctor unique provider identifier, National
        Provider Identifier (NPI) or reference uid based provider lookups. BetterDoctor
        identifiers and NPIs for doctors and practices can be discovered using BetterDoctor
        API???s search functionalities. <br><h4 style=''margin-bottom: 0px !important;''>
        Return Headers </h4> <div>Last-Modified: Timestamp of the last validation
        made over the matching validations. The value can be used to query changes
        in the validation status for the provider using since parameter in collaboration
        with HEAD method.</div>'
      operationId: the-endpoint-can-be-used-to-identify-providers-with-validation-data-the-search-supports-betterdoctor
      x-api-path-slug: validations-get
      parameters:
      - in: query
        name: data_type
        description: Provider type to search validations for
      - in: query
        name: data_uid
        description: Paired with data_type
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: npi
        description: Paired with data_type
      - in: query
        name: ref_uid
        description: Optional to data_type style queries
      - in: query
        name: since
        description: Limits validations returned to the validations after the given
          timestamp value (ISO 8601)
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: validation_method
        description: Limits validations returned to a validation method wanted
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
    head:
      summary: Check if new records exists
      description: 'The endpoint can be used to identify providers with validation
        data, and discover changes. It providers search functionalities like its GET
        method alternative, but does not return any validation data. Instead of the
        data itself, it returns 200 OK if matching validation documents based on the
        given query are found. And it returns 304 if no validation documents are found
        after the timestamp given using If-Modified-Since HTTP header or since parameter.
        <br><h4 style=''margin-bottom: 0px !important;''> Return Headers </h4> <div>Last-Modified:
        Timestamp of the last validation made over the matching validations. </div>'
      operationId: the-endpoint-can-be-used-to-identify-providers-with-validation-data-and-discover-changes-it-provider
      x-api-path-slug: validations-head
      parameters:
      - in: query
        name: data_type
        description: Provider type to search validations for
      - in: query
        name: data_uid
        description: Paired with data_type
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: npi
        description: Paired with data_type
      - in: query
        name: ref_uid
        description: Optional to data_type style queries
      - in: query
        name: since
        description: Limits validations returned to the validations after the given
          timestamp value (ISO 8601)
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      - in: query
        name: validation_method
        description: Limits validations returned to a validation method wanted
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
  /validations/{uid}:
    get:
      summary: Retrieve a specific record
      description: 'Returns requested validation document. The endpoint is a conveniece
        method to check status and accepted data of a specific validation, like after
        creation of a validation. The response consist of raw data from the validation
        event and related validation information. <br><h4 style=''margin-bottom: 0px
        !important;''> Return Headers </h4> <div>Last-Modified: Timestamp of the validation
        made.</div>'
      operationId: returns-requested-validation-document-the-endpoint-is-a-conveniece-method-to-check-status-and-accept
      x-api-path-slug: validationsuid-get
      parameters:
      - in: path
        name: uid
        description: Unique identifier of a validation document
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
    head:
      summary: Check if a specific record exists
      description: 'The endpoint can be used to discover if a validation document
        exists in the API. <br><h4 style=''margin-bottom: 0px !important;''> Return
        Headers </h4> <div>Last-Modified: Timestamp of the validation made.</div>'
      operationId: the-endpoint-can-be-used-to-discover-if-a-validation-document-exists-in-the-api-brh4-stylemarginbott
      x-api-path-slug: validationsuid-head
      parameters:
      - in: path
        name: uid
        description: Unique identifier of a validation document
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
      - Record
      - Search
      - Validations
---