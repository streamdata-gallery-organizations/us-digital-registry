---
swagger: "2.0"
info:
  title: U.S. Digital Registry Mobile App API
  description: Providing access to a directory of the mobile applications for federal
    agencies.
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
  /mobile_apps/{id}.json:
    get:
      summary: Mobile App
      description: This returns an mobile app based on an ID
      operationId: Api::V1::MobileApps#show
      parameters:
      - in: path
        name: id
        description: ID of the mobile app
      responses:
        200:
          description: OK
      tags:
      - mobile apps
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