{
  "info": {
    "name": "GIGANDCROWD Get Request Requestid Condition Condition Documents",
    "_postman_id": "1920e8d7-7ca2-448c-b3aa-13dae6509276",
    "description": "Get request requestid condition condition documents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "f03dd67b-b62e-41cd-a132-b780a84fca8a",
          "name": "getApiV1RequestRequestConditionConditionDocuments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/:requestId/condition/:condition/documents"
              ],
              "variable": [
                {
                  "id": "condition",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get request requestid condition condition documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d0c9a63-8802-4ca8-baa7-cae9898162eb"
            }
          ]
        }
      ]
    }
  ]
}