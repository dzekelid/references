---
swagger: "2.0"
x-collection-name: Google Genomics
x-complete: 0
info:
  title: Google Genomics API Search References
  description: |-
    Searches for references which match the given criteria.

    For the definitions of references and other genomics resources, see
    [Fundamentals of Google
    Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

    Implements
    [GlobalAllianceApi.searchReferences](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L146).
  contact:
    name: Google
    url: https://google.com
  version: v1
host: genomics.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/references/search:
    post:
      summary: Search References
      description: |-
        Searches for references which match the given criteria.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchReferences](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L146).
      operationId: genomics.references.search
      x-api-path-slug: v1referencessearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reference
  /v1/references/{referenceId}:
    get:
      summary: Get Reference
      description: |-
        Gets a reference.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.getReference](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L158).
      operationId: genomics.references.get
      x-api-path-slug: v1referencesreferenceid-get
      parameters:
      - in: path
        name: referenceId
        description: The ID of the reference
      responses:
        200:
          description: OK
      tags:
      - Reference
  /v1/references/{referenceId}/bases:
    get:
      summary: Get Reference Base
      description: |-
        Lists the bases in a reference, optionally restricted to a range.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.getReferenceBases](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L221).
      operationId: genomics.references.bases.list
      x-api-path-slug: v1referencesreferenceidbases-get
      parameters:
      - in: query
        name: end
        description: The end position (0-based, exclusive) of this query
      - in: query
        name: pageSize
        description: The maximum number of bases to return in a single page
      - in: query
        name: pageToken
        description: The continuation token, which is used to page through large result
          sets
      - in: path
        name: referenceId
        description: The ID of the reference
      - in: query
        name: start
        description: The start position (0-based) of this query
      responses:
        200:
          description: OK
      tags:
      - Reference
  /v1/referencesets/search:
    post:
      summary: Search Reference Set
      description: |-
        Searches for reference sets which match the given criteria.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.searchReferenceSets](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L71)
      operationId: genomics.referencesets.search
      x-api-path-slug: v1referencesetssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Reference Set
  /v1/referencesets/{referenceSetId}:
    get:
      summary: Get Reference Set
      description: |-
        Gets a reference set.

        For the definitions of references and other genomics resources, see
        [Fundamentals of Google
        Genomics](https://cloud.google.com/genomics/fundamentals-of-google-genomics)

        Implements
        [GlobalAllianceApi.getReferenceSet](https://github.com/ga4gh/schemas/blob/v0.5.1/src/main/resources/avro/referencemethods.avdl#L83).
      operationId: genomics.referencesets.get
      x-api-path-slug: v1referencesetsreferencesetid-get
      parameters:
      - in: path
        name: referenceSetId
        description: The ID of the reference set
      responses:
        200:
          description: OK
      tags:
      - Reference Set
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