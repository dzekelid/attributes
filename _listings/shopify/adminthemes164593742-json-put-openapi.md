---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Update a theme's attributes
  description: Update a theme's attributes.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/themes/164593742.json:
    put:
      summary: Update a theme's attributes
      description: Update a theme's attributes.
      operationId: putAdminThemes164593742.json
      x-api-path-slug: adminthemes164593742-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Themes
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