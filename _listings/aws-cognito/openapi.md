---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListRecords:
    get:
      summary: List Records
      description: Gets paginated records, optionally changed after a particular sync
        count for a dataset and identity.
      operationId: listRecords
      x-api-path-slug: actionlistrecords-get
      parameters:
      - in: query
        name: DatasetName
        description: A string of up to 128 characters
        type: string
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: LastSyncCount
        description: The last server sync count for this record
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to be returned
        type: string
      - in: query
        name: NextToken
        description: A pagination token for obtaining the next page of results
        type: string
      - in: query
        name: SyncSessionToken
        description: A token containing a session ID, identity ID, and expiration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
  /?Action=UpdateRecords:
    get:
      summary: Update Records
      description: Posts updates to records and adds and deletes records for a dataset
        and user.
      operationId: updateRecords
      x-api-path-slug: actionupdaterecords-get
      parameters:
      - in: query
        name: ClientContext
        description: Intended to supply a device ID that will populate the lastModifiedBy
          field referenced in other methods
        type: string
      - in: query
        name: DatasetName
        description: A string of up to 128 characters
        type: string
      - in: query
        name: IdentityId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
---