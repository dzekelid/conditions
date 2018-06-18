{
  "info": {
    "name": "Weather Underground Get Key Geolookup Conditions Q Ca San Francisco",
    "_postman_id": "17c6fece-0e55-4f10-8c43-e2fe10ca0df9",
    "description": "This example will return the geographical and current conditions for San Francisco, California",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Weather",
      "item": [
        {
          "id": "4506ea87-727d-4bc5-bbb0-d4effbb17d6b",
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
              "id": "3d8904e4-08dc-4a1d-9a2a-4bd7a9c7ad46"
            }
          ]
        },
        {
          "id": "7419294a-4b70-4616-97c6-d015dc9c4ef3",
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
              "id": "18bb5201-c73d-428e-83b0-30249ffd65c1"
            }
          ]
        },
        {
          "id": "b196db0a-51e3-49c1-ac3e-211047a2c542",
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
              "id": "b3207032-d663-49c1-b5da-d830e784efea"
            }
          ]
        },
        {
          "id": "fb6304b7-061e-4f88-aefe-fbcd7ff5e1e1",
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
              "id": "f9d38dbf-3ea1-4f27-9995-d7df394c6c40"
            }
          ]
        },
        {
          "id": "b3f04047-6858-4232-9fe4-27b21b622d37",
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
              "id": "d4cc54cd-5b90-471f-9a69-a86a8b678b3d"
            }
          ]
        },
        {
          "id": "b9cef6fc-b9b5-4a8f-8843-435717ed3932",
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
              "id": "320a277e-b5ec-4fc8-961e-36debf0722c3"
            }
          ]
        },
        {
          "id": "fd793605-2229-4047-ad98-1158ab09a553",
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
              "id": "765b2797-7e2b-40c3-a4ba-2fb1ac1eada9"
            }
          ]
        },
        {
          "id": "8f37f06e-6bd8-4a69-88cc-4a85c4543089",
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
              "id": "bc75539d-4c29-4e54-878d-c8ce16b7df5a"
            }
          ]
        },
        {
          "id": "7704aeb7-24cf-4415-8f34-b0e3c88f4f74",
          "name": "Get_Astronomy_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/astronomy/q/CA/San_Francisco.json"
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
            "description": "This example will return the Astronomy of San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b704e34d-9806-46c7-b4b1-1242bac3d607"
            }
          ]
        },
        {
          "id": "04beb735-2ced-4e1f-932e-2a9df5e69037",
          "name": "Get_forecast3_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/forecast/q/CA/San_Francisco.json"
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
            "description": "This example will return the 3 Day Forecast Summary for San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33f56cdd-8a02-4db6-8ed7-ecea489462a7"
            }
          ]
        },
        {
          "id": "226ef1cc-3e38-4e3c-a7a7-e0b0f7f11624",
          "name": "Get_almanac_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/almanac/q/CA/San_Francisco.json"
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
            "description": "This example will return Today's Average Highs/Lows and Record Highs/Lows for San Francisco, California."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f10f584b-8525-482d-a16e-a7d34187b1ce"
            }
          ]
        },
        {
          "id": "368cdc92-5046-4166-b417-cd8b962428db",
          "name": "Get_French_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/forecast/lang:FR/q/France/Paris.json"
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
            "description": "This example will return Current Conditions and a 3 day simple Forecast for Paris France in French. See documentation page for full list of language code options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d447588-589a-47c2-9e75-60c9e3ca553a"
            }
          ]
        },
        {
          "id": "13af8fba-cc0c-41de-abf6-352a838ef672",
          "name": "Get_Spanish_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/conditions/forecast/lang:SP/q/Spain/Alicante.json"
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
            "description": "This example will return Current Conditions and a 3 day simple Forecast for Alicante, Spain in Spanish. See documentation page for full list of language code options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a4ac43a-d16f-494c-8416-354821a18e9b"
            }
          ]
        },
        {
          "id": "90dae658-744f-4682-b87a-e3612640e5c6",
          "name": "Get_forecast10_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/forecast10day/q/CA/San_Francisco.json"
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
            "description": "This example will return the 10 Day Forecast Summary for San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92f37ca8-0f78-43c7-8833-8c00c930689c"
            }
          ]
        },
        {
          "id": "e9810d4c-f1e8-49fe-a925-c87c1e47f92b",
          "name": "Get_OneDay_hourly_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/hourly/q/CA/San_Francisco.json"
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
            "description": "This example will return a detailed hourly forecast for the 'next' 36 hours in San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d942f91-871e-49b9-ac64-2b1386423ee4"
            }
          ]
        },
        {
          "id": "49d36eb6-4bf9-4005-9678-874124eddf49",
          "name": "Get_satellite_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/satellite/q/CA/San_Francisco.json"
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
            "description": "This example will return URL's for satellite (visual and IR) images for San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "275f1940-9e34-46ab-a68d-3ebb28023ca7"
            }
          ]
        },
        {
          "id": "f92c08e6-2f36-4483-b2f9-30a39c6f6474",
          "name": "Get_radar_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/radar/image.gif?maxlat=42.35%26maxlon=-109.311%26minlat=39.27%26minlon=-114.644%26width=600%26height=480%26newmaps=0"
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
            "description": "This example will return dynamic radar image around Salt Lake City, UT with a transparent background. See Docs for all the options for creating these images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dce7605e-6107-4c26-a10f-034ee23cc249"
            }
          ]
        },
        {
          "id": "89b8f7ff-09d4-4ce8-ae7c-fc8e5b4b7d4a",
          "name": "Get_radar_example2_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/radar/image.gif?maxlat=42.35%26maxlon=-109.311%26minlat=39.27%26minlon=-114.644%26width=600%26height=480%26newmaps=1"
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
            "description": "This example will return dynamic radar image around Salt Lake City, UT with a Base Map background. See Docs for all the options for creating these images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f940f5c5-efda-4c9e-b3bf-a325b38787d5"
            }
          ]
        },
        {
          "id": "e31da154-f5fe-444f-b79d-b78fae62b8d2",
          "name": "Get_alerts_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/alerts/q/CA/San_Francisco.json"
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
            "description": "This example will return active severe alerts for San Francisco, California.    This request only works in the USA, Canada and Europe."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0affff9-4d9b-43cc-bef6-1a27b59b60b9"
            }
          ]
        },
        {
          "id": "806eb969-2032-41eb-be45-b08804ebc147",
          "name": "Get_Tide_example1_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/tide/q/CA/San_Francisco.json"
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
            "description": "This example will return 4 days of tides for San Francisco, California starting 'today'.    This request only works in the USA."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "818db778-6937-4066-9489-c8e0e5150600"
            }
          ]
        },
        {
          "id": "3abe615e-d7d3-4e41-bcc7-5c1bc6e1a27f",
          "name": "Get_Tide_example2_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/tide_20160312/q/CA/San_Francisco.json"
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
            "description": "This example will return 4 days of tides for San Francisco, California following March 3 2012.    This request only works in the USA."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35df1c4c-0f95-4423-bc8f-0f89cf98cc07"
            }
          ]
        },
        {
          "id": "f78fc319-0969-404a-82f4-4bd00e38d357",
          "name": "Get_Tide_RAW_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/rawtide_20160312/q/CA/San_Francisco.json"
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
            "description": "This example will return raw tide data for San Francisco, California on March 3 2016.    This request only works in the USA."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2289949-3d38-4650-bb14-9b56a1753dcd"
            }
          ]
        },
        {
          "id": "3f62bb87-028f-413a-9a7b-0e0bdd391845",
          "name": "Get_TenDay_hourly_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/hourly10day/q/CA/San_Francisco.json"
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
            "description": "This example will return a detailed hourly forecast for the next 10 days in San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d116d423-6782-4430-92d6-719414a6c004"
            }
          ]
        },
        {
          "id": "cec63b5b-638d-4f4a-8ba8-3c4231cf5f36",
          "name": "Get_yesterday_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/yesterday/q/CA/San_Francisco.json"
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
            "description": "This example will return yesterday's weather in San Francisco, California."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f19dfaf5-c87d-417d-bb0e-9c6791fe2df5"
            }
          ]
        },
        {
          "id": "7e53e7fc-c7bf-407f-9ae9-53acf8a91227",
          "name": "Get_Planner_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/planner_10051031/q/CA/San_Francisco.json"
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
            "description": "This example will return a Historical roll up of weather data in San Francisco from Oct 5 to Oct 31. An example application: http://www.wunderground.com/travelplanner/index.asp"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b5599b3-f7de-4966-95f3-aa23296f797d"
            }
          ]
        },
        {
          "id": "8c7f08fe-e720-4145-b92e-3419d9fa7669",
          "name": "Get_cams_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/webcams/q/CA/San_Francisco.json"
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
            "description": "This example will return URL's to webcam images in San Francisco, California.    It will also return information about the webcam, including it's location in Lat,Long coordinates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0737e6f6-2dd9-4e7b-a872-0d6289a30eee"
            }
          ]
        },
        {
          "id": "0181677f-a9c9-463e-b9db-43ab8da1354d",
          "name": "Get_radar_example3_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/animatedradar/image.gif?maxlat=42.35%26maxlon=-109.311%26minlat=39.27%26minlon=-114.644%26width=600%26height=480%26newmaps=1"
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
            "description": "This example will return dynamic animated radar image around Salt Lake City, UT with a base map background. See Docs for all the options for creating these images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8454a3b9-2157-4c9e-aff6-1d9bf805e833"
            }
          ]
        },
        {
          "id": "2e4ff613-811c-46cc-996a-9032d8653beb",
          "name": "Get_radar_example4_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/animatedradar/image.gif?maxlat=42.35%26maxlon=-109.311%26minlat=39.27%26minlon=-114.644%26width=600%26height=480%26newmaps=0"
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
            "description": "This example will return dynamic animated radar image around Salt Lake City, UT with a transparent background. See Docs for all the options for creating these images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14fb094d-ecdb-4ee2-8736-26ad0b6a427f"
            }
          ]
        },
        {
          "id": "e08240b2-2303-4809-bed3-7b44633e4c97",
          "name": "Get_History_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/history_20101018/q/SFO.json"
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
            "description": "This example will return historical data for San Francisco, California for the specified date.    If you search by zip or lat/long you will get nearest airport."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e2c4dd3-85ab-497e-961a-0362a6279fcc"
            }
          ]
        },
        {
          "id": "31754435-0e32-49c3-bf7b-ff08d6a5daa2",
          "name": "Get_History_example_pws_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/history_20101018/q/pws:KCASANFR14.json"
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
            "description": "This example will return historical data for a Personal Weather Station for the specified date.    The feature only works with JSON.    XML will come out soon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49d20f46-f645-483b-92a4-87d26f6aadd0"
            }
          ]
        },
        {
          "id": "f0e44a42-a2c7-458b-aeda-20d8d48bfb87",
          "name": "Get_Geolocate_current_example_",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.wunderground.com",
              "path": [
                "api",
                ":key/geolookup/conditions/q/CA/San_Francisco.json"
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
            "description": "This example will return the geographical and current conditions for San Francisco, California"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "704ea38d-2584-422e-921c-cd9516b3050d"
            }
          ]
        }
      ]
    }
  ]
}