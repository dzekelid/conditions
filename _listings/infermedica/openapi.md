swagger: "2.0"
x-collection-name: Infermedica
x-complete: 1
info:
  title: Infermedica
  description: empower-your-healthcare-services-with-intelligent-diagnostic-insights-of-infermedica-api-
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