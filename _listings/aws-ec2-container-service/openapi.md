---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteAttributes:
    get:
      summary: Delete Attributes
      description: Deletes one or more custom attributes from an Amazon ECS resource.
      operationId: deleteAttributes
      x-api-path-slug: actiondeleteattributes-get
      parameters:
      - in: query
        name: attributes
        description: The attributes to delete from your resource
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that contains the resource to apply            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /?Action=ListAttributes:
    get:
      summary: List Attributes
      description: |-
        Lists the attributes for Amazon ECS resources within a specified target type and
                    cluster.
      operationId: listAttributes
      x-api-path-slug: actionlistattributes-get
      parameters:
      - in: query
        name: attributeName
        description: The name of the attribute with which to filter the results
        type: string
      - in: query
        name: attributeValue
        description: The value of the attribute with which to filter results
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          to list attributes
        type: string
      - in: query
        name: maxResults
        description: The maximum number of cluster results returned by ListAttributes
          in            paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListAttributes
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      - in: query
        name: targetType
        description: The type of the target with which to list attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /?Action=PutAttributes:
    get:
      summary: Put Attributes
      description: Create or update an attribute on an Amazon ECS resource.
      operationId: putAttributes
      x-api-path-slug: actionputattributes-get
      parameters:
      - in: query
        name: attributes
        description: The attributes to apply to your resource
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that contains the resource to apply            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
---