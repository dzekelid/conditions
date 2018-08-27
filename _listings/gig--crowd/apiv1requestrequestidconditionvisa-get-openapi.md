---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Request Requestid Condition Visa
  version: 1.0.0
  description: Get request requestid condition visa.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/{requestId}/condition/visa:
    get:
      summary: Get Request Requestid Condition Visa
      description: Get request requestid condition visa.
      operationId: getApiV1RequestRequestConditionVisa
      x-api-path-slug: apiv1requestrequestidconditionvisa-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Visa
    post:
      summary: Post Request Requestid Condition Visa
      description: Post request requestid condition visa.
      operationId: postApiV1RequestRequestConditionVisa
      x-api-path-slug: apiv1requestrequestidconditionvisa-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Visa
  /api/v1/request/{requestId}/condition/travel:
    get:
      summary: Get Request Requestid Condition Travel
      description: Get request requestid condition travel.
      operationId: getApiV1RequestRequestConditionTravel
      x-api-path-slug: apiv1requestrequestidconditiontravel-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Travel
    post:
      summary: Post Request Requestid Condition Travel
      description: Post request requestid condition travel.
      operationId: postApiV1RequestRequestConditionTravel
      x-api-path-slug: apiv1requestrequestidconditiontravel-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Travel
  /api/v1/request/{requestId}/condition/residence:
    get:
      summary: Get Request Requestid Condition Resence
      description: Get request requestid condition resence.
      operationId: getApiV1RequestRequestConditionResence
      x-api-path-slug: apiv1requestrequestidconditionresidence-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Resence
    post:
      summary: Post Request Requestid Condition Resence
      description: Post request requestid condition resence.
      operationId: postApiV1RequestRequestConditionResence
      x-api-path-slug: apiv1requestrequestidconditionresidence-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Resence
  /api/v1/request/{requestId}/condition/delivery:
    get:
      summary: Get Request Requestid Condition Delivery
      description: Get request requestid condition delivery.
      operationId: getApiV1RequestRequestConditionDelivery
      x-api-path-slug: apiv1requestrequestidconditiondelivery-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Delivery
    post:
      summary: Post Request Requestid Condition Delivery
      description: Post request requestid condition delivery.
      operationId: postApiV1RequestRequestConditionDelivery
      x-api-path-slug: apiv1requestrequestidconditiondelivery-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Delivery
  /api/v1/request/{requestId}/condition/{condition}/confirm:
    post:
      summary: Post Request Requestid Condition Condition Confirm
      description: Post request requestid condition condition confirm.
      operationId: postApiV1RequestRequestConditionConditionConfirm
      x-api-path-slug: apiv1requestrequestidconditionconditionconfirm-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: condition
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Condition
      - Confirm
  /api/v1/request/{requestId}/condition/{condition}/reject:
    post:
      summary: Post Request Requestid Condition Condition Reject
      description: Post request requestid condition condition reject.
      operationId: postApiV1RequestRequestConditionConditionReject
      x-api-path-slug: apiv1requestrequestidconditionconditionreject-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: condition
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Condition
      - Reject
  /api/v1/request/{requestId}/condition/{condition}/documents:
    get:
      summary: Get Request Requestid Condition Condition Documents
      description: Get request requestid condition condition documents.
      operationId: getApiV1RequestRequestConditionConditionDocuments
      x-api-path-slug: apiv1requestrequestidconditionconditiondocuments-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: condition
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Condition
      - Documents
    post:
      summary: Post Request Requestid Condition Condition Documents
      description: Post request requestid condition condition documents.
      operationId: postApiV1RequestRequestConditionConditionDocuments
      x-api-path-slug: apiv1requestrequestidconditionconditiondocuments-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Condition
      - Documents
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