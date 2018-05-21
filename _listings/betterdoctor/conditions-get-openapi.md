---
swagger: "2.0"
x-collection-name: BetterDoctor
x-complete: 0
info:
  title: BetterDoctor Retrieve a list of known conditions
  description: List all conditions
  version: 1.0.0
host: api.betterdoctor.com
basePath: /2016-03-01
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conditions:
    get:
      summary: Retrieve a list of known conditions
      description: List all conditions
      operationId: list-all-conditions
      x-api-path-slug: conditions-get
      parameters:
      - in: query
        name: fields
        description: A comma-separated list of fields to include
      - in: query
        name: limit
        description: For paginated list operations; specifies the maximum number of
          items to retrieve
      - in: query
        name: skip
        description: For paginated list operations; specifies the zero-based start
          index of the first item to retrieve
      - in: query
        name: user_key
        description: Your API access key
      responses:
        200:
          description: OK
      tags:
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