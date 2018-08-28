{
  "info": {
    "name": "AWS Cognito API List Records",
    "_postman_id": "829594e6-c1bd-4b7d-9c15-2dc64dc002e0",
    "description": "Gets paginated records, optionally changed after a particular sync count for a dataset and identity.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Records",
      "item": [
        {
          "id": "578ac84b-9cdc-4c27-af0c-ab47fcbe775b",
          "name": "listRecords",
          "request": {
            "url": "http://example.com/api/?Action=ListRecords?DatasetName=DatasetName&IdentityId=IdentityId&IdentityPoolId=IdentityPoolId&LastSyncCount=LastSyncCount&MaxResults=MaxResults&NextToken=NextToken&SyncSessionToken=SyncSessionToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets paginated records, optionally changed after a particular sync count for a dataset and identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00915b27-4dd2-44f8-8b72-36332c1991ee"
            }
          ]
        }
      ]
    }
  ]
}