{
  "info": {
    "name": "BetterDoctor Retrieve a list of known conditions",
    "_postman_id": "fee06faf-4d93-4f26-af0d-7cf02cbe9f3a",
    "description": "List all conditions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conditions",
      "item": [
        {
          "id": "e74b32ea-5209-46fb-a99a-da45fd0d1bd7",
          "name": "list-all-conditions",
          "request": {
            "url": "http://api.betterdoctor.com/2016-03-01/conditions?fields=%7B%7D&limit=%7B%7D&skip=%7B%7D&user_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all conditions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09d94110-6abb-4b39-a984-e9039f3b80de"
            }
          ]
        }
      ]
    }
  ]
}