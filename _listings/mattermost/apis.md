---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: References
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Get the user's preferences
  x-api-slug: mattermost-api
  description: |-
    Get a list of the user's preferences.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences
  tags: Users,Preferences
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/mattermost/usersuser-idpreferences-get-openapi.md
- name: Mattermost API Save the user's preferences
  x-api-slug: mattermost-api
  description: |-
    Save a list of the user's preferences.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences
  tags: Save,Users,Preferences
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/mattermost/usersuser-idpreferences-put-openapi.md
- name: Mattermost API Delete user's preferences
  x-api-slug: mattermost-api
  description: |-
    Delete a list of the user's preferences.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences/delete
  tags: Users,Preferences
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/mattermost/usersuser-idpreferencesdelete-post-openapi.md
- name: Mattermost API List a user's preferences by category
  x-api-slug: mattermost-api
  description: |-
    Lists the current user's stored preferences in the given category.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4//users/{user_id}/preferences/{category}
  tags: List,Users,Preferences,By,Category
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/mattermost/usersuser-idpreferencescategory-get-openapi.md
- name: Mattermost API
  x-api-slug: mattermost-api
  description: Open source, private cloud Slack-alternative, Workplace messaging for
    web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
    configurable, and scalable from teams to the enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: References
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/mattermost/openapi.md
x-common:
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---