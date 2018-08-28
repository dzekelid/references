---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 0
info:
  title: LH Public Aircraft
  version: "1.0"
  description: List all aircraft types or one specific aircraft type.
host: api.lufthansa.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /references/aircraft/{aircraftCode}:
    get:
      summary: Aircraft
      description: List all aircraft types or one specific aircraft type.
      operationId: ReferencesAircraftByAircraftCodeGet
      x-api-path-slug: referencesaircraftaircraftcode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: aircraftCode
        description: 3-character IATA aircraft code
      - in: query
        name: limit
        description: Number of records returned per request
      - in: query
        name: offset
        description: Number of records skipped
      responses:
        200:
          description: OK
      tags:
      - References
      - Aircraft
      - AircraftCode
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