---
swagger: "2.0"
x-collection-name: Lufthansa
x-complete: 1
info:
  title: LH Public
  version: "1.0"
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
  /references/airlines/{airlineCode}:
    get:
      summary: Airlines
      description: List all airlines or one specific airline.
      operationId: ReferencesAirlinesByAirlineCodeGet
      x-api-path-slug: referencesairlinesairlinecode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airlineCode
        description: 2-character IATA airline/carrier code
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
      - Airlines
      - AirlineCode
  /references/airports/nearest/{latitude},{longitude}:
    get:
      summary: Nearest Airports
      description: List the 5 closest airports to the given latitude and longitude,
        irrespective of the radius of the reference point.
      operationId: ReferencesAirportsNearestByLatitudeAndLongitudeGet
      x-api-path-slug: referencesairportsnearestlatitudelongitude-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: query
        name: lang
        description: 2 letter ISO 3166-1 language code
      - in: path
        name: latitude
        description: Latitude in decimal format to at most 3 decimal places
      - in: path
        name: longitude
        description: Longitude in decimal format to at most 3 decimal places
      responses:
        200:
          description: OK
      tags:
      - References
      - Airports
      - Nearest
      - Latitude
      - Longitude
  /references/airports/{airportCode}:
    get:
      summary: Airports
      description: List all airports or one specific airport. All airports response
        is very large. It is possible to request the response in a specific language.
      operationId: ReferencesAirportsByAirportCodeGet
      x-api-path-slug: referencesairportsairportcode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: airportCode
        description: 3-letter IATA airport code
      - in: query
        name: lang
        description: 2-letter ISO 3166-1 language code
      - in: query
        name: LHoperated
        description: Restrict the results to locations with flights operated by LH
          (false=0, true=1)
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
      - Airports
      - AirportCode
  /references/cities/{cityCode}:
    get:
      summary: Cities
      description: List all cities or one specific city. It is possible to request
        the response in a specific language.
      operationId: ReferencesCitiesByCityCodeGet
      x-api-path-slug: referencescitiescitycode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: cityCode
        description: 3-letter IATA city code
      - in: query
        name: lang
        description: 2 letter ISO 3166-1 language code
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
      - Cities
      - CityCode
  /references/countries/{countryCode}:
    get:
      summary: Countries
      description: List all countries or one specific country. It is possible to request
        the response in a specific language.
      operationId: ReferencesCountriesByCountryCodeGet
      x-api-path-slug: referencescountriescountrycode-get
      parameters:
      - in: header
        name: Accept
        description: 'http header: application/json or application/xml (Acceptable
          values are: application/json, application/xml)'
      - in: path
        name: countryCode
        description: 2-letter ISO 3166-1 country code
      - in: query
        name: lang
        description: 2 letter ISO 3166-1 language code
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
      - Countries
      - CountryCode
---