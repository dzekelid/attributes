---
swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
---