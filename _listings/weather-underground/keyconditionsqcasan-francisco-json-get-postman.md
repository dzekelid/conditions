{
  "info": {
    "name": "Weather Underground Get Key Conditions Q Ca San Francisco",
    "_postman_id": "77bfe2e9-260b-4e04-8766-9179edd22b09",
    "description": "This example will return the current conditions in San Francisco, California",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Weather",
      "item": [
        {
          "id": "a4c0e6ae-fe17-480a-a61b-d730bce1e638",
          "name": "Get_USA_Geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/CA/San_Francisco.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the geographic attributes of San Francisco CA.    Use {2 letter state code} /    {City Name}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae435c68-491a-4b47-95b8-cce9067a4e0e"
            }
          ]
        },
        {
          "id": "ae0405a0-200f-4f90-a8eb-9443821a7d55",
          "name": "Get_Outside_of_USA_Geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/France/Paris.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the geographic attributes of Paris, France. Use {Full Country Name} / {City Name}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "898c455a-502c-4867-aed6-5ea01f037039"
            }
          ]
        },
        {
          "id": "5dfaf3ef-7232-4286-ac41-f258f8f9a85f",
          "name": "Get_IPAddress_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/autoip.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the geographic attributes associated with the IP address location of the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12c4fed9-aa59-4dfc-b1ae-23ea9a4345b1"
            }
          ]
        },
        {
          "id": "a999c769-75fa-49ba-b23f-4b682f6d76dd",
          "name": "Get_ZIP_geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/94107.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the geographic attributes of zip code 94107"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "855e6f95-98bb-4875-ac74-999aefea67af"
            }
          ]
        },
        {
          "id": "42e97d36-83c1-4ff4-9c31-fa7798790fa8",
          "name": "Get_Airport_geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/SFO.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the geographic attributes of San Francisco International Airport (Airport Code: SFO)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1b95889-e14a-4053-a6bb-83d18b583afd"
            }
          ]
        },
        {
          "id": "f7a84c22-bd68-49e3-a9ea-b069baf71628",
          "name": "Get_Lat_Long_geolocate_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/q/37.776289,-122.395234.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the the geographic attributes of Latitude 37.776289 N, Longitude 122.395234 W"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99faea1d-9f82-4fef-ad11-add9aabc3f31"
            }
          ]
        },
        {
          "id": "6d4de84d-c0d0-491a-b359-4772d939315c",
          "name": "Get_pws_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/q/pws:KCATAHOE2.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the the current weather conditions at the Personal Weather Station (pws) KCATAHOE2"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ceb42fc9-8b46-4cf5-bbc4-d79aa4128dcb"
            }
          ]
        },
        {
          "id": "92e84168-74a7-4503-8c37-50a132565356",
          "name": "Get_Conditions_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/q/CA/San_Francisco.json"
              ],
              "variable": [
                {
                  "id": "key",
                  "value": "key",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This example will return the current conditions in San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7fabc899-ee79-4ffe-9a84-6c674bb754a6"
            }
          ]
        }
      ]
    }
  ]
}