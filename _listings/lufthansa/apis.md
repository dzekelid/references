---
name: Lufthansa
x-slug: lufthansa
description: Book your flights to Germany, Italy, UK or France online at attractive
  low fares. Fly via Frankfurt, Munich or Zurich - Lufthansa United States of America
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
x-kinRank: "7"
x-alexaRank: "3886"
tags: References
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/apis.md
specificationVersion: "0.14"
apis:
- name: LH Public - Aircraft
  x-api-slug: referencesaircraftaircraftcode-get
  description: List all aircraft types or one specific aircraft type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesaircraftaircraftcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesaircraftaircraftcode-get-openapi.md
- name: LH Public - Airlines
  x-api-slug: referencesairlinesairlinecode-get
  description: List all airlines or one specific airline.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairlinesairlinecode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairlinesairlinecode-get-openapi.md
- name: LH Public - Nearest Airports
  x-api-slug: referencesairportsnearestlatitudelongitude-get
  description: List the 5 closest airports to the given latitude and longitude, irrespective
    of the radius of the reference point.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsnearestlatitudelongitude-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsnearestlatitudelongitude-get-openapi.md
- name: LH Public - Airports
  x-api-slug: referencesairportsairportcode-get
  description: List all airports or one specific airport. All airports response is
    very large. It is possible to request the response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsairportcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencesairportsairportcode-get-openapi.md
- name: LH Public - Cities
  x-api-slug: referencescitiescitycode-get
  description: List all cities or one specific city. It is possible to request the
    response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescitiescitycode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescitiescitycode-get-openapi.md
- name: LH Public - Countries
  x-api-slug: referencescountriescountrycode-get
  description: List all countries or one specific country. It is possible to request
    the response in a specific language.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28453-lh-partner.jpg
  humanURL: http://lufthansa.com
  baseURL: https://api.lufthansa.com//v1
  tags: Airlines, API Provider, Profiles, General Data, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescountriescountrycode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/lufthansa/referencescountriescountrycode-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://lota.data.api.gallery.streamdata.io
- type: x-api-stack
  url: http://lufthansa.stack.network
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