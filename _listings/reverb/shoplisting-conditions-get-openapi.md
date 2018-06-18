---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: reverb Get Shop Listing Conditions
  description: List of supported product conditions
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listing_conditions:
    get:
      summary: Get Listing Conditions
      description: List of supported product conditions
      operationId: getListingConditions
      x-api-path-slug: listing-conditions-get
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Conditions
  /shop/listing_conditions:
    get:
      summary: Get Shop Listing Conditions
      description: List of supported product conditions
      operationId: getShopListingConditions
      x-api-path-slug: shoplisting-conditions-get
      responses:
        200:
          description: OK
      tags:
      - Shop
      - Listing
      - Conditions
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---