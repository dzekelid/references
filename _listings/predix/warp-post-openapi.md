---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Dynamic Time Warping Warp subject and reference arrays
  description: Warp subject and reference arrays.
  version: 1.0.0
host: time-series-service-doc.grc-apps.svc.ice.ge.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /warp:
    post:
      summary: Warp subject and reference arrays
      description: Warp subject and reference arrays.
      operationId: postWarp
      x-api-path-slug: warp-post
      parameters:
      - in: body
        name: body
        description: Subject and Reference arrays to be processed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Warp
      - Subject
      - Reference
      - Arrays
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