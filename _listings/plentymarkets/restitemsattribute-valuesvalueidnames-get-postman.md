{
  "info": {
    "name": "Plentymarkets Get name and language for an attribute value ID",
    "_postman_id": "dfaae86b-fda3-4961-bb98-7bac878321cf",
    "description": "Gets name and language for an attribute value ID. The attribute value ID must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "c3b20701-1408-4212-9447-53f7ee9bbd58",
          "name": "getRestItemsAttributes",
          "request": {
            "url": "http://example.com/rest/items/attributes?updatedAt=%7B%7D&with=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists all attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4696df0e-5698-4293-a03d-bdf2ad2072f4"
            }
          ]
        }
      ]
    },
    {
      "name": "Name",
      "item": [
        {
          "id": "9b948247-615e-4ff1-8d1c-b207632317ee",
          "name": "getRestItemsAttributeValuesValueNames",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/attribute_values/:valueId/names"
              ],
              "variable": [
                {
                  "id": "valueId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets name and language for an attribute value ID. The attribute value ID must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f39a96c7-58d4-454d-a5a6-e1c9f2044933"
            }
          ]
        }
      ]
    }
  ]
}