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
  /tags/{id}.json:
    get:
      summary: Tag
      description: This returns a tag based on an ID
      operationId: Api::V1::Tags#show
      parameters:
      - in: path
        name: id
        description: ID of the tag
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