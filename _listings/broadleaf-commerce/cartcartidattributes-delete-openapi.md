---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Delete Cart Attributes
  description: Delete cart attributes.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /cart/{cartId}/attributes:
    put:
      summary: Put Cart Attributes
      description: Put cart attributes.
      operationId: putCartCartAttributes
      x-api-path-slug: cartcartidattributes-put
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
      - Attributes
    delete:
      summary: Delete Cart Attributes
      description: Delete cart attributes.
      operationId: deleteCartCartAttributes
      x-api-path-slug: cartcartidattributes-delete
      parameters:
      - in: path
        name: cartId
        description: cartId
      - in: query
        name: customerId
      - in: query
        name: priceOrder
        description: priceOrder
      - in: body
        name: requestParams
        description: requestParams
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cart
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