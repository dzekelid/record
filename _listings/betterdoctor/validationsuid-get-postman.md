{
  "info": {
    "name": "BetterDoctor Retrieve a specific record",
    "_postman_id": "4b1b153a-ef19-41f0-b756-cdea8ce7c327",
    "description": "Returns requested validation document. The endpoint is a conveniece method to check status and accepted data of a specific validation, like after creation of a validation. The response consist of raw data from the validation event and related validation information. <br><h4 style='margin-bottom: 0px !important;'> Return Headers </h4> <div>Last-Modified: Timestamp of the validation made.</div>",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "record",
      "item": [
        {
          "id": "78ce99c9-5ea7-486c-a5a8-b0151faed81b",
          "name": "returns-requested-validation-document-the-endpoint-is-a-conveniece-method-to-check-status-and-accept",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.betterdoctor.com",
              "path": [
                "2016-03-01",
                "validations/:uid"
              ],
              "query": [
                {
                  "key": "user_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "uid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns requested validation document"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6474703-3047-4e70-9755-f9a24eb480c4"
            }
          ]
        }
      ]
    }
  ]
}