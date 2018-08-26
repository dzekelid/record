{
  "info": {
    "name": "Dezrez Record and timestamp a visit to a 'page' on Rezi.",
    "_postman_id": "86ae9923-713a-4920-a9ba-042120c9390f",
    "description": "Record and timestamp a visit to a 'page' on rezi..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Record",
      "item": [
        {
          "id": "436b1d4c-a000-463f-aafb-3d82f0e7ed31",
          "name": "Stats_RecordVisitBypageTypeByentityIdByroleId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/stats/RecordVisit/:pageType/:entityId"
              ],
              "query": [
                {
                  "key": "roleId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "entityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "pageType",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Record and timestamp a visit to a 'page' on rezi.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d8b6719-9248-4cde-bc00-31d0c5df9c91"
            }
          ]
        }
      ]
    }
  ]
}