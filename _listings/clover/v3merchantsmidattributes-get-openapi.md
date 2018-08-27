---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get all attributes
  version: 1.0.0
  description: See the description for 'get all item groups'.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/attributes:
    get:
      summary: Get all attributes
      description: See the description for 'get all item groups'.
      operationId: GetAttributes
      x-api-path-slug: v3merchantsmidattributes-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, name, id, deletedTime, itemGroup'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Attributes
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