{
  "info": {
    "name": "Plentymarkets Lists all attribute maps.",
    "_postman_id": "a4269af7-17d1-4fc0-92a2-089d635b34a0",
    "description": "Lists all attribute maps..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "b26c094c-acf1-4349-b281-4bbc3cf53e23",
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
              "id": "a14b98a6-fbae-4909-b1e5-58aed1f9be64"
            }
          ]
        }
      ]
    }
  ]
}