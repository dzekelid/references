---
swagger: "2.0"
x-collection-name: SugarSync
x-complete: 0
info:
  title: Sugar Sync  API Creating a Refresh Token
  description: An application needs to be authorized to access a users SugarSync resources
    through the Platform API.nTo do that, the app needs to create a refresh token.
    When a user first runs the application, it creates a refresh tokennby submitting
    a POST request that includes the users credentials to the API.nIf the request
    is successful, the SugarSync service grants the application permission to access
    the users account and returns a refresh token.n
  version: "1"
host: api.sugarsync.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /app-authorization:
    post:
      summary: Creating a Refresh Token
      description: An application needs to be authorized to access a users SugarSync
        resources through the Platform API.nTo do that, the app needs to create a
        refresh token. When a user first runs the application, it creates a refresh
        tokennby submitting a POST request that includes the users credentials to
        the API.nIf the request is successful, the SugarSync service grants the application
        permission to access the users account and returns a refresh token.n
      operationId: creating-a-refresh-token
      x-api-path-slug: appauthorization-post
      parameters:
      - in: header
        name: Content-Length
        description: The length of the request body
      - in: header
        name: Content-Type
        description: The content type and character encoding of the response
      - in: header
        name: Host
        description: The domain name of the server
      - in: header
        name: User-Agent
        description: The client application implementing the network protocol for
          communication between          the client and server
      responses:
        1:
          description: Photoset not found - The photoset id passed was not the id
            of avalid photoset owned by the calling user
        2:
          description: Photo not found - The photo id passed was not the id of a valid
            photo owned by the calling user
        95:
          description: SSL is required - SSL is required to access the Flickr API
        96:
          description: Invalid signature - The passed signature was invalid
        97:
          description: Missing signature - The call required signing but no signature
            was sent
        98:
          description: Login failed / Invalid auth token - The login details or auth
            token passed were invalid
        99:
          description: User not logged in / Insufficient permissions - The method
            requires user authentication but the user was not logged in, or the authenticated
            method call did not have the required permissions
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
        "":
          description: ""
        400:
          description: Bad input parameter
        401:
          description: Bad or expired token
        403:
          description: Bad OAuth request (wrong consumer key, bad nonce, expired timestamp
        404:
          description: File or folder not found at the specified path
        405:
          description: Request method not expected (generally should be GET or POST)
        429:
          description: Your app is making too many requests and is being rate limited
        503:
          description: If the response includes the Retry-After header, this means
            your OAuth 1
        507:
          description: User is over Dropbox storage quota
        5xx:
          description: Server error
        200:
          description: OK
      tags:
      - App
      - Authorization
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