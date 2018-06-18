---
name: Weather Underground
x-slug: weather-underground
description: Weather Underground provides local & long range weather forecasts, weather
  reports, maps & tropical weather conditions for locations worldwide.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
x-kinRank: "10"
x-alexaRank: "619"
tags: Conditions
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/apis.md
specificationVersion: "0.14"
apis:
- name: Weather Underground Get Key Conditions Q Pws Kcatahoe2
  x-api-slug: weather-underground
  description: This example will return the the current weather conditions at the
    Personal Weather Station (pws) KCATAHOE2
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/conditions/q/pws:KCATAHOE2.json
  tags: Weather,Key,Conditions,Q,Pws:KCATAHOE2,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsqpwskcatahoe2-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsqpwskcatahoe2-json-get-openapi.md
- name: Weather Underground Get Key Conditions Q Ca San Francisco
  x-api-slug: weather-underground
  description: This example will return the current conditions in San Francisco, California
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/conditions/q/CA/San_Francisco.json
  tags: Weather,Key,Conditions,Q,CA,San,Francisco,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsqcasan-francisco-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsqcasan-francisco-json-get-openapi.md
- name: Weather Underground Get Key Conditions Forecast Lang Fr Q France Paris
  x-api-slug: weather-underground
  description: This example will return Current Conditions and a 3 day simple Forecast
    for Paris France in French. See documentation page for full list of language code
    options.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/conditions/forecast/lang:FR/q/France/Paris.json
  tags: Weather,Key,Conditions,Forecast,Lang:FR,Q,France,Paris,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsforecastlangfrqfranceparis-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsforecastlangfrqfranceparis-json-get-openapi.md
- name: Weather Underground Get Key Conditions Forecast Lang Sp Q Spain Alicante
  x-api-slug: weather-underground
  description: This example will return Current Conditions and a 3 day simple Forecast
    for Alicante, Spain in Spanish. See documentation page for full list of language
    code options.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/conditions/forecast/lang:SP/q/Spain/Alicante.json
  tags: Weather,Key,Conditions,Forecast,Lang:SP,Q,Spain,Alicante,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsforecastlangspqspainalicante-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keyconditionsforecastlangspqspainalicante-json-get-openapi.md
- name: Weather Underground Get Key Geolookup Conditions Q Ca San Francisco
  x-api-slug: weather-underground
  description: This example will return the geographical and current conditions for
    San Francisco, California
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/geolookup/conditions/q/CA/San_Francisco.json
  tags: Weather,Key,Geolookup,Conditions,Q,CA,San,Francisco,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keygeolookupconditionsqcasan-francisco-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keygeolookupconditionsqcasan-francisco-json-get-openapi.md
- name: Weather Underground Get Key Geolookup Conditions Forecast Q Ca San Francisco
  x-api-slug: weather-underground
  description: This example will return the geographical, current conditions and 3
    day forecast summary for San Francisco, California
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/geolookup/conditions/forecast/q/CA/San_Francisco.json
  tags: Weather,Key,Geolookup,Conditions,Forecast,Q,CA,San,Francisco,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keygeolookupconditionsforecastqcasan-francisco-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/keygeolookupconditionsforecastqcasan-francisco-json-get-openapi.md
- name: Weather Underground
  x-api-slug: weather-underground
  description: Weather Underground provides local & long range weather forecasts,
    weather reports, maps & tropical weather conditions for locations worldwide.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api/
  tags: Conditions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/weather-underground/openapi.md
x-common:
- type: x-application-gallery
  url: http://www.wunderground.com/weather/api/d/featured_applications.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/weather-underground
- type: x-crunchbase
  url: http://www.crunchbase.com/company/weather-underground
- type: x-developer
  url: http://www.wunderground.com/weather/api
- type: x-email
  url: help@wunderground.com
- type: x-email
  url: press@wunderground.com
- type: x-email
  url: ademail@wunderground.com
- type: x-email
  url: wuhelp@wunderground.com
- type: x-forum
  url: http://www.wunderground.com/weather/api/d/community.html
- type: x-knowledgebase
  url: http://help.wunderground.com/knowledgebase
- type: x-pricing
  url: http://www.wunderground.com/weather/api/d/pricing.html
- type: x-privacy
  url: http://www.wunderground.com/members/tos.asp#privacy
- type: x-selfservice-registration
  url: http://www.wunderground.com/weather/api/d/login.html
- type: x-terms-of-service
  url: http://www.wunderground.com/members/tos.asp
- type: x-twitter
  url: https://twitter.com/wunderground
- type: x-twitter
  url: https://twitter.com/weatherapi
- type: x-website
  url: http://www.wunderground.com
- type: x-website
  url: http://wunderground.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---