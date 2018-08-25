{
  "info": {
    "name": "Plentymarkets List attributes",
    "_postman_id": "759d4f17-bb3d-4090-b492-870a81ed931d",
    "description": "Lists all attributes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "59a60158-d161-433b-8e50-4695cea68983",
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
              "id": "088d6f45-7e32-4e83-89e9-f02b606399ee"
            }
          ]
        }
      ]
    }
  ]
}