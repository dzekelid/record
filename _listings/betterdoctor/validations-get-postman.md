{
  "info": {
    "name": "BetterDoctor Record search",
    "_postman_id": "6f4d67a3-8323-4a22-8410-5d9e9018f69a",
    "description": "The endpoint can be used to identify providers with validation data. The search supports BetterDoctor unique provider identifier, National Provider Identifier (NPI) or reference uid based provider lookups. BetterDoctor identifiers and NPIs for doctors and practices can be discovered using BetterDoctor API???s search functionalities. <br><h4 style='margin-bottom: 0px !important;'> Return Headers </h4> <div>Last-Modified: Timestamp of the last validation made over the matching validations. The value can be used to query changes in the validation status for the provider using since parameter in collaboration with HEAD method.</div>",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "record",
      "item": [
        {
          "id": "0763b05e-707c-4ff3-9f54-945921f7f6bb",
          "name": "the-endpoint-can-be-used-to-identify-providers-with-validation-data-the-search-supports-betterdoctor",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/validations?data_type=%7B%7D&data_uid=%7B%7D&limit=%7B%7D&npi=%7B%7D&ref_uid=%7B%7D&since=%7B%7D&skip=%7B%7D&user_key=%7B%7D&validation_method=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The endpoint can be used to identify providers with validation data"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b35011d7-e135-455e-b0cb-9dfcf0391ffc"
            }
          ]
        }
      ]
    }
  ]
}