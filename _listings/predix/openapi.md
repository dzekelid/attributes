swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/connector/resource:
    get:
      summary: Retrieves connector configuration for external resource attributes
        for the given zone.
      description: Retrieves connector configuration for external resource attributes
        for the given zone..
      operationId: getResourceConnectorUsingGET_1
      x-api-path-slug: v1connectorresource-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
    put:
      summary: Creates or updates connector configuration for external resource attributes
        for the given zone.
      description: Creates or updates connector configuration for external resource
        attributes for the given zone..
      operationId: putResourceConnectorUsingPUT_1
      x-api-path-slug: v1connectorresource-put
      parameters:
      - in: body
        name: connector
        description: New or updated connector configuration for external resource
          attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Updates
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
    delete:
      summary: Deletes connector configuration for external resource attributes for
        the given zone.
      description: Deletes connector configuration for external resource attributes
        for the given zone..
      operationId: deleteResourceConnectorUsingDELETE
      x-api-path-slug: v1connectorresource-delete
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Connector
      - Configurationexternal
      - Resource
      - Attributesthe
      - Given
      - Zone
  /v1/connector/subject:
    get:
      summary: Retrieves connector configuration for external subject attributes for
        the given zone.
      description: Retrieves connector configuration for external subject attributes
        for the given zone..
      operationId: getSubjectConnectorUsingGET
      x-api-path-slug: v1connectorsubject-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
    put:
      summary: Creates or updates connector configuration for external subject attributes
        for the given zone.
      description: Creates or updates connector configuration for external subject
        attributes for the given zone..
      operationId: putSubjectConnectorUsingPUT_1
      x-api-path-slug: v1connectorsubject-put
      parameters:
      - in: body
        name: connector
        description: New or updated connector configuration for external subject attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - Updates
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
    delete:
      summary: Deletes connector configuration for external subject attributes for
        the given zone.
      description: Deletes connector configuration for external subject attributes
        for the given zone..
      operationId: deleteSubjectConnectorUsingDELETE
      x-api-path-slug: v1connectorsubject-delete
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Connector
      - Configurationexternal
      - Subject
      - Attributesthe
      - Given
      - Zone
  /decks/{id}:
    put:
      summary: Update attributes for a Tag instance and persist it.
      description: Update attributes for a tag instance and persist it..
      operationId: putDecks
      x-api-path-slug: decksid-put
      parameters:
      - in: body
        name: data
        description: An object of Deck property name/value pairs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Attributesa
      - Tag
      - Instance
      - Persist
      - It
  /cards/{id}:
    put:
      summary: Update attributes for a Card instance and persist it.
      description: Update attributes for a card instance and persist it..
      operationId: putCards
      x-api-path-slug: cardsid-put
      parameters:
      - in: body
        name: data
        description: An object of Card property name/value pairs
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: PersistedModel id
      responses:
        200:
          description: OK
      tags:
      - Attributesa
      - Card
      - Instance
      - Persist
      - It