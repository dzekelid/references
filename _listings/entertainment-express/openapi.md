swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /TvMedia/reference/lineups:
    get:
      summary: ""
      description: Get list of generic lineup IDs that can be used.  A 'generic' lineup
        is not a real lineup, but a collection of stations defined by TV Media.  Any
        listing retrieved using a generic lineup will not return any channel number
        information, as it is irrelevant.
      operationId: GetTvMediaGenericLineups
      x-api-path-slug: tvmediareferencelineups-get
      parameters:
      - in: query
        name: Detail
        description: Set level of detail for response
      - in: query
        name: TvMediaApiKey
        description: API Key supplied by TvMedia
      responses:
        200:
          description: OK
      tags:
      - TvMedia
      - Reference
      - Lineups