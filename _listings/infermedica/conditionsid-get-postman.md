{
  "info": {
    "name": "Infermedica Get Conditions",
    "_postman_id": "e994ed71-f65a-4564-b864-84a28b793460",
    "description": "Returns details of a single condition specified by id parameter.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Healthcare",
      "item": [
        {
          "id": "323adc88-63cb-4f86-8f51-000d227d0421",
          "name": "getConditions",
          "request": {
            "url": "http://api.infermedica.com/v1/conditions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all available conditions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae0b1c97-328d-4b32-a764-f639409d5e30"
            }
          ]
        },
        {
          "id": "36a3c3fe-2e6a-4812-830c-fb2ff3992e5c",
          "name": "getConditions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.infermedica.com",
              "path": [
                "v1",
                "conditions/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns details of a single condition specified by id parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ec5b957-08f8-47d7-bc9e-60f03ea2e2d7"
            }
          ]
        }
      ]
    }
  ]
}