---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get Category Attributes
  description: Get category attributes.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/settings:
    get:
      summary: Get Settings Attributes
      description: Get settings attributes.
      operationId: V2SettingsGet2
      x-api-path-slug: v2settings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Settings
      - Attributes
  /v2/integrations/attributes:
    get:
      summary: Get Integration Attributes
      description: Get integration attributes.
      operationId: V2IntegrationsAttributesGet
      x-api-path-slug: v2integrationsattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Integration
      - Attributes
  /v2/brands/attributes:
    get:
      summary: Get Brand Attributes
      description: Get brand attributes.
      operationId: V2BrandsAttributesGet
      x-api-path-slug: v2brandsattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Attributes
  /categories/attributes:
    get:
      summary: Get Category Attributes
      description: Get category attributes.
      operationId: CategoriesAttributesGet
      x-api-path-slug: categoriesattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
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