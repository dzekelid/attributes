{
  "info": {
    "name": "Plentymarkets Lists all attribute value maps.",
    "_postman_id": "7b25b231-05eb-4da4-a8f8-59febf51d856",
    "description": "Lists all attribute value maps..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "bb27f46b-7a3b-4aca-b0af-cd632ce3db5a",
          "name": "getRestItemsAttributesMaps",
          "request": {
            "url": "http://example.com/rest/items/attributes/maps",
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
            "description": "Lists all attribute maps.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2ab7115-c527-491b-b97c-926451796feb"
            }
          ]
        },
        {
          "id": "a07d8e72-82ae-4005-9811-580b0d29a33f",
          "name": "getRestItemsAttributesValuesMaps",
          "request": {
            "url": "http://example.com/rest/items/attributes/values/maps",
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
            "description": "Lists all attribute value maps.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6af079c6-3bf8-4581-aa7c-0d9e5e5dae6b"
            }
          ]
        }
      ]
    }
  ]
}