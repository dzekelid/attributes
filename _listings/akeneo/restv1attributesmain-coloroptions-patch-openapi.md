---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API attribute options (2.1 only)
  description: Assuming that the given code is the code of an existing attribute
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/attributes:
    get:
      summary: attributes
      description: Attributes.
      operationId: RestV1AttributesGet
      x-api-path-slug: restv1attributes-get
      responses:
        200:
          description: OK
      tags:
      - Attributes
    patch:
      summary: attributes
      description: Attributes.
      operationId: RestV1AttributesPatch
      x-api-path-slug: restv1attributes-patch
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
      - Attributes
    post:
      summary: attribute
      description: Assuming that there is no "new_attribute" already existing
      operationId: RestV1AttributesPost
      x-api-path-slug: restv1attributes-post
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
      - Attribute
  /rest/v1/attributes/auto_exposure:
    get:
      summary: attribute
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesAutoExposureGet
      x-api-path-slug: restv1attributesauto-exposure-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
    patch:
      summary: attribute
      description: Attribute.
      operationId: RestV1AttributesAutoExposurePatch
      x-api-path-slug: restv1attributesauto-exposure-patch
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
      - Attribute
  /rest/v1/attributes/main_color/options/white:
    get:
      summary: attribute option
      description: Assuming that the given codes are respectively the code of an existing
        attribute and an existing option of this attribute
      operationId: RestV1AttributesMainColorOptionsWhiteGet
      x-api-path-slug: restv1attributesmain-coloroptionswhite-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Option
    patch:
      summary: attribute option
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesMainColorOptionsWhitePatch
      x-api-path-slug: restv1attributesmain-coloroptionswhite-patch
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
      - Attribute
      - Option
  /rest/v1/attributes/main_color/options:
    get:
      summary: attribute options
      description: Attribute options.
      operationId: RestV1AttributesMainColorOptionsGet
      x-api-path-slug: restv1attributesmain-coloroptions-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Options
    post:
      summary: attribute option
      description: Assuming that there is no "yellow" option already existing for
        the given attribute
      operationId: RestV1AttributesMainColorOptionsPost
      x-api-path-slug: restv1attributesmain-coloroptions-post
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
      - Attribute
      - Option
    patch:
      summary: attribute options (2.1 only)
      description: Assuming that the given code is the code of an existing attribute
      operationId: RestV1AttributesMainColorOptionsPatch
      x-api-path-slug: restv1attributesmain-coloroptions-patch
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
      - Attribute
      - Options
      - (2
      - "1"
      - Only)
  /rest/v1/attribute-groups/technical:
    get:
      summary: attribute group (2.x only)
      description: Assuming that the given code is the code of an existing attribute
        group
      operationId: RestV1AttributeGroupsTechnicalGet
      x-api-path-slug: restv1attributegroupstechnical-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Group
      - (2
      - X
      - Only)
    patch:
      summary: attribute group (2.x only)
      description: Attribute group (2.x only).
      operationId: RestV1AttributeGroupsTechnicalPatch
      x-api-path-slug: restv1attributegroupstechnical-patch
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
      - Attribute
      - Group
      - (2
      - X
      - Only)
  /rest/v1/attribute-groups:
    get:
      summary: attribute groups (2.x only)
      description: Attribute groups (2.x only).
      operationId: RestV1AttributeGroupsGet
      x-api-path-slug: restv1attributegroups-get
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Groups
      - (2
      - X
      - Only)
    post:
      summary: attribute group (2.x only)
      description: Assuming that there is no "new_attribute_group" already existing
      operationId: RestV1AttributeGroupsPost
      x-api-path-slug: restv1attributegroups-post
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
      - Attribute
      - Group
      - (2
      - X
      - Only)
    patch:
      summary: attribute groups (2.x only)
      description: Attribute groups (2.x only).
      operationId: RestV1AttributeGroupsPatch
      x-api-path-slug: restv1attributegroups-patch
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
      - Attribute
      - Groups
      - (2
      - X
      - Only)
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