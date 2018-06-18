---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 0
info:
  title: Infermedica Get Conditions
  description: Returns details of a single condition specified by id parameter.
  version: v2
host: api.infermedica.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conditions:
    get:
      summary: Get Conditions
      description: Returns a list of all available conditions.
      operationId: getConditions
      x-api-path-slug: conditions-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Conditions
  /conditions/{id}:
    get:
      summary: Get Conditions
      description: Returns details of a single condition specified by id parameter.
      operationId: getConditions
      x-api-path-slug: conditionsid-get
      parameters:
      - in: path
        name: id
        description: condition id
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Conditions
      - Id
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