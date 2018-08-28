---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Refundsettings
  version: 1.0.0
  description: Get api refundsettings.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/RefundAddress:
    get:
      summary: Get API Refundaddress
      description: Get api refundaddress.
      operationId: ApiRefundAddressGet
      x-api-path-slug: apirefundaddress-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Refundaddress
    post:
      summary: Add API Refundaddress
      description: Add api refundaddress.
      operationId: ApiRefundAddressPost
      x-api-path-slug: apirefundaddress-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: body
        name: refundAddressModel
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Refundaddress
  /api/RefundSettings:
    get:
      summary: Get API Refundsettings
      description: Get api refundsettings.
      operationId: ApiRefundSettingsGet
      x-api-path-slug: apirefundsettings-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Refundsettings
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