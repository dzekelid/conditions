{
  "info": {
    "name": "Infermedica Get Conditions",
    "_postman_id": "be246e27-c034-43f1-bfc4-b0a135399f77",
    "description": "Returns a list of all available conditions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Healthcare",
      "item": [
        {
          "id": "6cc30d32-c920-4d0b-8d43-0e14edcb4415",
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
              "id": "ce810838-ffa1-4e4f-af6d-db33c800f65b"
            }
          ]
        }
      ]
    }
  ]
}