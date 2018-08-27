---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Updates an attribute value map.
  description: Updates an attribute value map. The ID of the attribute, the ID of
    the attribute value and the ID of the market must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/attributes:
    get:
      summary: List attributes
      description: Lists all attributes.
      operationId: getRestItemsAttributes
      x-api-path-slug: restitemsattributes-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified attribute information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Attributes
    post:
      summary: Create an attribute
      description: Creates an attribute.
      operationId: postRestItemsAttributes
      x-api-path-slug: restitemsattributes-post
      parameters:
      - in: body
        name: /rest/items/attributes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Attribute
  /rest/items/attribute_values/{valueId}/names:
    get:
      summary: Get name and language for an attribute value ID
      description: Gets name and language for an attribute value ID. The attribute
        value ID must be specified.
      operationId: getRestItemsAttributeValuesValueNames
      x-api-path-slug: restitemsattribute-valuesvalueidnames-get
      parameters:
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Name
      - Languagean
      - Attribute
      - Value
      - ID
    post:
      summary: Create an attribute value name
      description: Creates an attribute value name.
      operationId: postRestItemsAttributeValuesValueNames
      x-api-path-slug: restitemsattribute-valuesvalueidnames-post
      parameters:
      - in: body
        name: /rest/items/attribute_values/{valueId}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
  /rest/items/attribute_values/{valueId}/names/{lang}:
    delete:
      summary: Delete an attribute value name
      description: Deletes an attribute value name. The attribute value ID and language
        must be specified.
      operationId: deleteRestItemsAttributeValuesValueNamesLang
      x-api-path-slug: restitemsattribute-valuesvalueidnameslang-delete
      parameters:
      - in: path
        name: lang
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
    get:
      summary: Get an attribute value name
      description: Gets the attribute value name. The attribute value ID and language
        must be specified.
      operationId: getRestItemsAttributeValuesValueNamesLang
      x-api-path-slug: restitemsattribute-valuesvalueidnameslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
    put:
      summary: Update an attribute value name
      description: Updates an attribute value name.
      operationId: putRestItemsAttributeValuesValueNamesLang
      x-api-path-slug: restitemsattribute-valuesvalueidnameslang-put
      parameters:
      - in: body
        name: /rest/items/attribute_values/{valueId}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: lang
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Name
  /rest/items/attributes/maps:
    get:
      summary: Lists all attribute maps.
      description: Lists all attribute maps..
      operationId: getRestItemsAttributesMaps
      x-api-path-slug: restitemsattributesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Maps
  /rest/items/attributes/markets/maps:
    post:
      summary: Creates a new attribute map.
      description: Creates a new attribute map..
      operationId: postRestItemsAttributesMarketsMaps
      x-api-path-slug: restitemsattributesmarketsmaps-post
      parameters:
      - in: body
        name: /rest/items/attributes/markets/maps
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Attribute
      - Map
  /rest/items/attributes/values/maps:
    get:
      summary: Lists all attribute value maps.
      description: Lists all attribute value maps..
      operationId: getRestItemsAttributesValuesMaps
      x-api-path-slug: restitemsattributesvaluesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Value
      - Maps
  /rest/items/attributes/values/markets/maps:
    post:
      summary: Creates a new attribute value map.
      description: Creates a new attribute value map..
      operationId: postRestItemsAttributesValuesMarketsMaps
      x-api-path-slug: restitemsattributesvaluesmarketsmaps-post
      parameters:
      - in: body
        name: /rest/items/attributes/values/markets/maps
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Attribute
      - Value
      - Map
  /rest/items/attributes/{attributeId}/markets/{marketId}/maps:
    delete:
      summary: Deletes an attribute map.
      description: Deletes an attribute map. The ID of the attribute and the ID of
        the market must be specified.
      operationId: deleteRestItemsAttributesAttributeMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidmarketsmarketidmaps-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Map
    get:
      summary: Gets an attribute map.
      description: Gets an attribute map. The ID of the attribute and the ID of the
        market must be specified.
      operationId: getRestItemsAttributesAttributeMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidmarketsmarketidmaps-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Map
    put:
      summary: Updates an attribute map.
      description: Updates an attribute map. The ID of the attribute and the ID of
        the market must be specified.
      operationId: putRestItemsAttributesAttributeMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidmarketsmarketidmaps-put
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Map
  /rest/items/attributes/{attributeId}/names:
    get:
      summary: Get an attribute name
      description: Gets the attribute name in the specified language. The language
        code must be specified.
      operationId: getRestItemsAttributesAttributeNames
      x-api-path-slug: restitemsattributesattributeidnames-get
      parameters:
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
    post:
      summary: Create an attribute name
      description: Creates an attribute name in the specified language. The language
        code must be specified.
      operationId: postRestItemsAttributesAttributeNames
      x-api-path-slug: restitemsattributesattributeidnames-post
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
  /rest/items/attributes/{attributeId}/names/{lang}:
    delete:
      summary: Delete an attribute name
      description: Deletes the attribute name in the specified language. The language
        code and attribute name must be specified.
      operationId: deleteRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
    get:
      summary: List attribute names
      description: Lists the attribute names of an attribute.
      operationId: getRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Names
    put:
      summary: Update an attribute name
      description: Updates the attribute name in the specified language. The language
        code and attribute name must be specified.
      operationId: putRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-put
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/names/{lang}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Name
  /rest/items/attributes/{attributeId}/value_market_names:
    get:
      summary: Search attribute value market names
      description: Search attribute value market names.
      operationId: getRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lang
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referenceType
      responses:
        200:
          description: OK
      tags:
      - Search
      - Attribute
      - Value
      - Market
      - Names
    post:
      summary: Create an attribute value market name
      description: Creates an attribute value market name.
      operationId: postRestItemsAttributesAttributeValueMarketNames
      x-api-path-slug: restitemsattributesattributeidvalue-market-names-post
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/value_market_names
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
  /rest/items/attributes/{attributeId}/value_market_names/{valueId}/{lang}/{referenceType}:
    delete:
      summary: Delete an attribute value market name
      description: Deletes an attribute value market name. The attribute value ID
        and language must be specified.
      operationId: deleteRestItemsAttributesAttributeValueMarketNamesValueLangReferencetype
      x-api-path-slug: restitemsattributesattributeidvalue-market-namesvalueidlangreferencetype-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      - in: path
        name: referenceType
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
    put:
      summary: Update an attribute value market name
      description: Updates an attribute value market name. The attribute value ID
        and language must be specified.
      operationId: putRestItemsAttributesAttributeValueMarketNamesValueLangReferencetype
      x-api-path-slug: restitemsattributesattributeidvalue-market-namesvalueidlangreferencetype-put
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/value_market_names/{valueId}/{lang}/{referenceType}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      - in: path
        name: lang
      - in: path
        name: referenceType
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Market
      - Name
  /rest/items/attributes/{attributeId}/values:
    get:
      summary: List attribute values
      description: Lists the attribute values for an attribute. The attribute ID must
        be specified.
      operationId: getRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvalues-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified attribute value information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Values
    post:
      summary: Create an attribute value
      description: Creates an attribute value.
      operationId: postRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvalues-post
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/values
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
  /rest/items/attributes/{attributeId}/values/{attributeValueId}/markets/{marketId}/maps:
    delete:
      summary: Deletes an attribute value map.
      description: Deletes an attribute value map. The ID of the attribute, the ID
        of the attribute value and the ID of the market must be specified.
      operationId: deleteRestItemsAttributesAttributeValuesAttributevalueMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidvaluesattributevalueidmarketsmarketidmaps-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: attributeValueId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Value
      - Map
    get:
      summary: Gets an attribute value map.
      description: Gets an attribute value map. The ID of the attribute, the ID of
        the attribute value and the ID of the market must be specified.
      operationId: getRestItemsAttributesAttributeValuesAttributevalueMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidvaluesattributevalueidmarketsmarketidmaps-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: attributeValueId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Value
      - Map
    put:
      summary: Updates an attribute value map.
      description: Updates an attribute value map. The ID of the attribute, the ID
        of the attribute value and the ID of the market must be specified.
      operationId: putRestItemsAttributesAttributeValuesAttributevalueMarketsMarketMaps
      x-api-path-slug: restitemsattributesattributeidvaluesattributevalueidmarketsmarketidmaps-put
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: attributeValueId
      - in: path
        name: marketId
      responses:
        200:
          description: OK
      tags:
      - S
      - Attribute
      - Value
      - Map
  /rest/items/attributes/{attributeId}/values/{id}:
    delete:
      summary: Delete an attribute value
      description: Deletes an attribute value. The attribute ID must be specified.
      operationId: deleteRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvaluesid-delete
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
    get:
      summary: Get an attribute value
      description: Get an attribute value. The ID of the attribute value must be specified.
      operationId: getRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvaluesid-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: id
      - in: query
        name: with
        description: Includes the specified attribute value information in the results
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
    put:
      summary: Update an attribute value
      description: Updates an attribute value. The attribute value must be specified.
      operationId: putRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvaluesid-put
      parameters:
      - in: body
        name: /rest/items/attributes/{attributeId}/values/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: attributeId
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
  /rest/items/attributes/{id}:
    delete:
      summary: Delete an attribute
      description: Deletes an attribute. The ID of the attribute must be specified.
      operationId: deleteRestItemsAttributes
      x-api-path-slug: restitemsattributesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
    get:
      summary: Get an attribute
      description: Gets an attribute. The ID of the attribute must be specified.
      operationId: getRestItemsAttributes
      x-api-path-slug: restitemsattributesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: Includes the specified attribute information in the results
      responses:
        200:
          description: OK
      tags:
      - Attribute
    put:
      summary: Update an attribute
      description: Updates an attribute. The ID of the attribute must be specified.
      operationId: putRestItemsAttributes
      x-api-path-slug: restitemsattributesid-put
      parameters:
      - in: body
        name: /rest/items/attributes/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Attribute
  /rest/items/{id}/images/attribute_value_markets:
    get:
      summary: List attribute value image link
      description: Lists the images linked to an attribute value.
      operationId: getRestItemsImagesAttributeValueMarkets
      x-api-path-slug: restitemsidimagesattribute-value-markets-get
      parameters:
      - in: query
        name: attributeId
        description: The unique ID of the attribute
      - in: path
        name: id
      - in: query
        name: imageId
        description: The unique ID of the image
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: query
        name: valueId
        description: The unique ID of the attribute value
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/{imageId}/attribute_value_markets:
    post:
      summary: Create an attribute value image link
      description: Creates a link between an image and an attribute value.
      operationId: postRestItemsImagesImageAttributeValueMarkets
      x-api-path-slug: restitemsidimagesimageidattribute-value-markets-post
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/attribute_value_markets
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/{imageId}/attribute_value_markets/{valueId}:
    delete:
      summary: Delete an attribute value image link
      description: Deletes the link between an image and an attribute value. The attribute
        ID must be specified.
      operationId: deleteRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
    get:
      summary: Get an attribute value image link
      description: 'Gets an attribute value image link. The following IDs must be
        specified: image ID, item ID and value ID.'
      operationId: getRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
    put:
      summary: Update an attribute value image link
      description: 'Updates the link between an image and an attribute value. The
        following IDs must be specified: image ID, item ID and value ID.'
      operationId: putRestItemsImagesImageAttributeValueMarketsValue
      x-api-path-slug: restitemsidimagesimageidattribute-value-marketsvalueid-put
      parameters:
      - in: body
        name: /rest/items/{id}/images/{imageId}/attribute_value_markets/{valueId}
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: attributeId
        description: The unique ID of the attribute
      - in: path
        name: id
      - in: path
        name: imageId
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: path
        name: valueId
      responses:
        200:
          description: OK
      tags:
      - Attribute
      - Value
      - Image
      - Link
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