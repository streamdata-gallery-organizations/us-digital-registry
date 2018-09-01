---
swagger: "2.0"
x-collection-name: US Digital Registry
x-complete: 0
info:
  title: U.S. Digital Registry Tag API Tag
  description: This returns a tag based on an ID.
  version: 1.0.0
host: usdigitalregistry.digitalgov.gov
basePath: /api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /agencies.json:
    get:
      summary: Agencies
      description: This lists all active agencies in the system. These agencies can
        be used to query for social media accounts, mobile products, and galleries.
      operationId: Api::V1::Agencies#index
      x-api-path-slug: agencies-json-get
      parameters:
      - in: query
        name: no_accounts
        description: Including this parameter with value true will cause the endpoint
          to include agencies that have no account in the system
        type: string
        format: string
      - in: query
        name: page
        description: Page number
      - in: query
        name: page_size
        description: Number of results per page
      - in: query
        name: q
        description: String to compare to the name & acronym of the agencies
      responses:
        200:
          description: OK
      tags:
      - Agencies
  /agencies/{id}.json:
    get:
      summary: Agency
      description: This returns an agency based on an ID.
      operationId: Api::V1::Agencies#show
      x-api-path-slug: agenciesid-json-get
      parameters:
      - in: path
        name: id
        description: ID of the agency
      responses:
        200:
          description: OK
      tags:
      - Agencies
  /mobile_apps/tokeninput.json:
    get:
      summary: Mobile App Token
      description: This returns tokens representing agencies, tags, and a basic text
        search token for the purpose of building search dialogs
      operationId: Api::V1::MobileApps#tokeninput
      x-api-path-slug: mobile-appstokeninput-json-get
      parameters:
      - in: query
        name: q
        description: String to compare to the various values
      responses:
        200:
          description: OK
      tags:
      - Mobile Apps
  /mobile_apps.json:
    get:
      summary: Mobile Apps
      description: This lists all active mobile apps.  It accepts parameters to perform
        basic search as well as searching by tag and agency.
      operationId: Api::V1::MobileApps#index
      x-api-path-slug: mobile-apps-json-get
      parameters:
      - in: query
        name: agencies
        description: Comma separated list of agency ids
      - in: query
        name: language
        description: Language of the social media accounts to return
      - in: query
        name: page
        description: Page number
      - in: query
        name: page_size
        description: Number of results per page, defaults to 25
      - in: query
        name: q
        description: String to compare to the name & short description of the mobile
          apps
      - in: query
        name: tags
        description: Comma separated list of tag ids
      responses:
        200:
          description: OK
      tags:
      - Mobile Apps
  /mobile_apps/{id}.json:
    get:
      summary: Mobile App
      description: This returns an mobile app based on an ID.
      operationId: Api::V1::MobileApps#show
      x-api-path-slug: mobile-appsid-json-get
      parameters:
      - in: path
        name: id
        description: ID of the mobile app
      responses:
        200:
          description: OK
      tags:
      - Mobile Apps
  /social_media/verify.json:
    get:
      summary: Social Media Verify
      description: This returns an agency based on an URL. If not found, it will return
        a 404
      operationId: Api::V1::SocialMedia#verify
      x-api-path-slug: social-mediaverify-json-get
      parameters:
      - in: query
        name: url
        description: URL of social media account
      responses:
        200:
          description: OK
      tags:
      - Social Media
  /social_media/services.json:
    get:
      summary: Social Media Services
      description: This returns a list of services along with the number of accounts
        registered with them
      operationId: Api::V1::SocialMedia#services
      x-api-path-slug: social-mediaservices-json-get
      responses:
        200:
          description: OK
      tags:
      - Social Media
  /social_media/tokeninput.json:
    get:
      summary: Social Media Token
      description: This returns tokens representing services, agencies, tags, and
        a basic text search token for the purpose of building search dialogs
      operationId: Api::V1::SocialMedia#tokeninput
      x-api-path-slug: social-mediatokeninput-json-get
      parameters:
      - in: query
        name: q
        description: String to compare to the various values
      responses:
        200:
          description: OK
      tags:
      - Social Media
  /social_media.json:
    get:
      summary: Social Media
      description: This lists all active accounts. It accepts parameters to perform
        basic search as well as search by service, agency, or tags.
      operationId: Api::V1::SocialMedia#index
      x-api-path-slug: social-media-json-get
      parameters:
      - in: query
        name: agencies
        description: Comma separated list of agency ids
      - in: query
        name: language
        description: Language of the social media accounts to return
      - in: query
        name: page
        description: Page number
      - in: query
        name: page_size
        description: Number of results per page, defaults to 25
      - in: query
        name: q
        description: String to compare to the name of accounts
      - in: query
        name: services
        description: Comma separated list of service keys (available via services
          call)
      - in: query
        name: tags
        description: Comma separated list of tag ids
      responses:
        200:
          description: OK
      tags:
      - Social Media
  /social_media/{id}.json:
    get:
      summary: Social Media
      description: This returns an agency based on an ID.
      operationId: Api::V1::SocialMedia#show
      x-api-path-slug: social-mediaid-json-get
      parameters:
      - in: path
        name: id
        description: ID of the account
      responses:
        200:
          description: OK
      tags:
      - Social Media
  /tags/types.json:
    get:
      summary: Tag Types
      description: This returns a tag based on an ID.
      operationId: Api::V1::Tags#types
      x-api-path-slug: tagstypes-json-get
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags.json:
    get:
      summary: Tags
      description: This lists all tags.  It accepts parameters to perform basic search.
      operationId: Api::V1::Tags#index
      x-api-path-slug: tags-json-get
      parameters:
      - in: query
        name: page
        description: Page number
      - in: query
        name: page_size
        description: Number of results per page
      - in: query
        name: q
        description: String to compare to the short name of tags
      - in: query
        name: type
        description: Comma separated list of tag types
      responses:
        200:
          description: OK
      tags:
      - Tags
  /tags/{id}.json:
    get:
      summary: Tag
      description: This returns a tag based on an ID.
      operationId: Api::V1::Tags#show
      x-api-path-slug: tagsid-json-get
      parameters:
      - in: path
        name: id
        description: ID of the tag
      responses:
        200:
          description: OK
      tags:
      - Tags
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