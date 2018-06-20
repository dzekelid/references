---
name: Lufthansa
x-slug: lufthansa
description: Book your flights to Germany, Italy, UK or France online at attractive
  low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
x-kinRank: "7"
x-alexaRank: "3886"
tags: References
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/apis.md
specificationVersion: "0.14"
apis:
- name: LH Public Aircraft
  x-api-slug: lh-public
  description: List all aircraft types or one specific aircraft type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//references/aircraft/{aircraftCode}
  tags: References,Aircraft,AircraftCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesaircraftaircraftcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesaircraftaircraftcode-get-openapi.md
- name: LH Public Airlines
  x-api-slug: lh-public
  description: List all airlines or one specific airline.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//references/airlines/{airlineCode}
  tags: References,Airlines,AirlineCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairlinesairlinecode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairlinesairlinecode-get-openapi.md
- name: LH Public Nearest Airports
  x-api-slug: lh-public
  description: List the 5 closest airports to the given latitude and longitude, irrespective
    of the radius of the reference point.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//references/airports/nearest/{latitude},{longitude}
  tags: References,Airports,Nearest,Latitude,Longitude
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsnearestlatitudelongitude-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsnearestlatitudelongitude-get-openapi.md
- name: LH Public Airports
  x-api-slug: lh-public
  description: List all airports or one specific airport. All airports response is
    very large. It is possible to request the response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//references/airports/{airportCode}
  tags: References,Airports,AirportCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsairportcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsairportcode-get-openapi.md
- name: LH Public Cities
  x-api-slug: lh-public
  description: List all cities or one specific city. It is possible to request the
    response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//references/cities/{cityCode}
  tags: References,Cities,CityCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescitiescitycode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescitiescitycode-get-openapi.md
- name: LH Public Countries
  x-api-slug: lh-public
  description: List all countries or one specific country. It is possible to request
    the response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1//references/countries/{countryCode}
  tags: References,Countries,CountryCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescountriescountrycode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescountriescountrycode-get-openapi.md
- name: LH Public
  x-api-slug: lh-public
  description: Book your flights to Germany, Italy, UK or France online at attractive
    low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: References
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/lufthansa
- type: x-twitter
  url: https://twitter.com/lufthansa
- type: x-website
  url: http://lufthansa.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---