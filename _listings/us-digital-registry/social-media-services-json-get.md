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
  /social_media/services.json:
    get:
      summary: Social Media Services
      description: This returns a list of services along with the number of accounts
        registered with them
      operationId: Api::V1::SocialMedia#services
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