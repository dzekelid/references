swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
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