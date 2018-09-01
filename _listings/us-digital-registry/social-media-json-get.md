---
swagger: "2.0"
info:
  title: U.S. Digital Registry Social Media API
  description: Provides access to the social media accounts for top federal agencies.
  version: 1.0.0
host: usdigitalregistry.digitalgov.gov
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /social_media.json:
    get:
      summary: Social Media
      description: This lists all active accounts
      operationId: Api::V1::SocialMedia#index
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
      - social media
definitions: []
x-collection-name: U.S. Digital Registry
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