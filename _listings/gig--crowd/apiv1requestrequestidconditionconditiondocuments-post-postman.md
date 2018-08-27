{
  "info": {
    "name": "GIGANDCROWD Post Request Requestid Condition Condition Documents",
    "_postman_id": "5936b2ca-e79e-4abd-957a-0ce5a46bdae5",
    "description": "Post request requestid condition condition documents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "378f3fc1-e6a5-4dba-a20f-05356361db19",
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
              "id": "7efc744c-524c-4467-a51a-f596f02e3e80"
            }
          ]
        },
        {
          "id": "c526e935-c3a7-4f1e-bc89-db5302bb9432",
          "name": "postApiV1RequestRequestConditionConditionDocuments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/:requestId/condition/:condition/documents"
              ],
              "query": [
                {
                  "key": "file",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "requestId",
                  "value": "requestId",
                  "type": "string"
                },
                {
                  "id": "condition",
                  "value": "condition",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
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
            "description": "Post request requestid condition condition documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "110e4253-71f5-47eb-964a-6e51dde35c52"
            }
          ]
        }
      ]
    }
  ]
}