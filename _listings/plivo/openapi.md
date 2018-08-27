swagger: "2.0"
x-collection-name: Plivo
x-complete: 1
info:
  title: Plivo
  version: 1.0.0
host: api.plivo.com
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/{id}/attribute:
    delete:
      summary: Delete Account Attribute
      description: Remove attribute from an account. Attribute name is used as a quary
        parameter. For this API request account/owner, system/admin or system/manager
        role is required
      operationId: removeAttribute
      x-api-path-slug: accountidattribute-delete
      parameters:
      - in: path
        name: id
        description: Account ID
      - in: query
        name: name
        description: Attribute name to be removed
      responses:
        200:
          description: OK
      tags:
      - Account
      - Id
      - Attribute