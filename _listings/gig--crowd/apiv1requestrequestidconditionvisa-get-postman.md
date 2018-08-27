{
  "info": {
    "name": "GIGANDCROWD Get Request Requestid Condition Visa",
    "_postman_id": "fcd49433-f205-4de1-b3a2-0e2b0e802092",
    "description": "Get request requestid condition visa.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "a5e5a648-b8de-45bf-8cec-4a4f70a790ff",
          "name": "getApiV1RequestRequestConditionVisa",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/:requestId/condition/visa"
              ],
              "variable": [
                {
                  "id": "requestId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
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
            "description": "Get request requestid condition visa."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7126f94f-21d0-4ff9-bffa-5d18089b59d2"
            }
          ]
        }
      ]
    }
  ]
}