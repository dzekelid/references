---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: References
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Users API Update multiple preferences
  x-api-slug: instructure-canvas-users-api
  description: Update multiple preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preferences
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferences-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferences-put-openapi.md
- name: Instructure Canvas Users API Update a preference
  x-api-slug: instructure-canvas-users-api
  description: Update a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preferences/notification
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put-openapi.md
- name: Instructure Canvas Users API Update multiple preferences
  x-api-slug: instructure-canvas-users-api
  description: Update multiple preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{type}/address/notification_preferences
  tags: Users,Self,Communication,Channels,Type,Address,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferences-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferences-put-openapi.md
- name: Instructure Canvas Users API Update a preference
  x-api-slug: instructure-canvas-users-api
  description: Update a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{type}/address/notification_preferences/{notification}
  tags: Users,Self,Communication,Channels,Type,Address,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put-openapi.md
- name: Instructure Canvas Users API List preferences
  x-api-slug: instructure-canvas-users-api
  description: List preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preferences
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get-openapi.md
- name: Instructure Canvas Users API Get a preference
  x-api-slug: instructure-canvas-users-api
  description: Get a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preferences/{notification}
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get-openapi.md
- name: Instructure Canvas Users API List preferences
  x-api-slug: instructure-canvas-users-api
  description: List preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}/notification_preferences
  tags: Users,User,Id,Communication,Channels,Type,Address,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferences-get-openapi.md
- name: Instructure Canvas Users API Get a preference
  x-api-slug: instructure-canvas-users-api
  description: Get a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}/notification_preferences/notification
  tags: Users,User,Id,Communication,Channels,Type,Address,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferencesnotification-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferencesnotification-get-openapi.md
- name: Instructure Canvas Users API
  x-api-slug: instructure-canvas-users-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: References
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/references/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---