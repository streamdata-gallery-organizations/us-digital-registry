---
swagger: "2.0"
info:
  title: U.S. Digital Registry Tag API
  description: Provides a access to the list of tags applied to federal government
    agencies and their social media accounts.
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
  /tags.json:
    get:
      summary: Tags
      description: This lists all tags
      operationId: Api::V1::Tags#index
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
      - in: type
        name: type
        description: Comma separated list of tag types
      responses:
        200:
          description: OK
      tags:
      - tags
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