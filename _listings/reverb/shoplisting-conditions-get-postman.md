{
  "info": {
    "name": "reverb Get Shop Listing Conditions",
    "_postman_id": "e1aef49e-b63b-4578-b582-8b79d03b0ff0",
    "description": "List of supported product conditions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Listing",
      "item": [
        {
          "id": "ca582290-e98b-4843-beca-920846c5393a",
          "name": "getListingConditions",
          "request": {
            "url": "http://api.reverb.com/api/listing_conditions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of supported product conditions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c867d80-538f-4a7b-be90-5023a2e3d57e"
            }
          ]
        }
      ]
    },
    {
      "name": "Shop",
      "item": [
        {
          "id": "ab1aa9fe-5c01-45cb-9b9f-00f1b141c062",
          "name": "getShopListingConditions",
          "request": {
            "url": "http://api.reverb.com/api/shop/listing_conditions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of supported product conditions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4484617-8a7d-444f-8e3b-b8297f3903f7"
            }
          ]
        }
      ]
    }
  ]
}