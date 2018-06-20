---
name: GlobalChange.gov
x-slug: globalchange-gov
description: The U.S. Global Change Research Program (USGCRP) was established by Presidential
  Initiative in 1989 and mandated by Congress in the Global Change Research Act (GCRA)
  of 1990 to &ldquo;assist the Nation and the world to understand, assess, predict,
  and respond to human-induced and natural processes of global change.&rdquo;
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
x-kinRank: "8"
x-alexaRank: "0"
tags: References
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/apis.md
specificationVersion: "0.14"
apis:
- name: Global Change Information System API List references.
  x-api-slug: global-change-information-system-api
  description: List the references, 20 per page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov////reference
  tags: References
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/reference-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/reference-get-openapi.md
- name: Global Change Information System API List references in a chapter
  x-api-slug: global-change-information-system-api
  description: Get a list of references in a chapter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov////report/{report_identifier}/chapter/{chapter_identifier}/reference
  tags: References,Chapter
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/reportreport-identifierchapterchapter-identifierreference-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/reportreport-identifierchapterchapter-identifierreference-get-openapi.md
- name: Global Change Information System API List references in a report.
  x-api-slug: global-change-information-system-api
  description: List the references in a report, 20 per page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov////report/{report_identifier}/reference
  tags: References,Report
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/reportreport-identifierreference-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/reportreport-identifierreference-get-openapi.md
- name: Global Change Information System API
  x-api-slug: global-change-information-system-api
  description: The U.S. Global Change Research Program (USGCRP) was established by
    Presidential Initiative in 1989 and mandated by Congress in the Global Change
    Research Act (GCRA) of 1990 to &ldquo;assist the Nation and the world to understand,
    assess, predict, and respond to human-induced and natural processes of global
    change.&rdquo;
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/global-change-gov.png
  humanURL: http://globalchange.gov/
  baseURL: https://data.globalchange.gov//
  tags: References
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/globalchange-gov/openapi.md
x-common:
- type: x-developer
  url: http://data.globalchange.gov/
- type: x-website
  url: http://globalchange.gov/
- type: x-website
  url: http://globalchange.gov
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---