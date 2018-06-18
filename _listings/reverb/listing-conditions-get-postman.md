{
  "info": {
    "name": "reverb Get Listing Conditions",
    "_postman_id": "c04ce61f-17fb-4b4b-a6c8-f2a9a420d0bd",
    "description": "List of supported product conditions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Listing",
      "item": [
        {
          "id": "bc7fb6d7-d4de-4c14-94c2-574c53a82c1f",
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
              "id": "3fa6b55d-984a-48e8-9d1e-fdd01b0c42bd"
            }
          ]
        }
      ]
    }
  ]
}