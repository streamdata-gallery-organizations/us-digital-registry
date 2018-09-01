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
  /social_media/tokeninput.json:
    get:
      summary: Social Media Token
      description: This returns tokens representing services, agencies, tags, and
        a basic text search token for the purpose of building search dialogs
      operationId: Api::V1::SocialMedia#tokeninput
      parameters:
      - in: query
        name: q
        description: String to compare to the various values
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