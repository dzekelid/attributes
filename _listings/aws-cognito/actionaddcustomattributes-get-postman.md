{
  "info": {
    "name": "AWS Cognito API Add Custom Attributes",
    "_postman_id": "d90332cb-f980-4332-a9f5-aa75f1442a43",
    "description": "Adds additional user attributes to the user pool schema.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes",
      "item": [
        {
          "id": "a5a1c058-0052-4d0a-a1b6-4d9b9fdf19dd",
          "name": "addCustomAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AddCustomAttributes?CustomAttributes=CustomAttributes&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds additional user attributes to the user pool schema."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "621aba5b-f3f8-419f-98e3-94b532bf8549"
            }
          ]
        }
      ]
    }
  ]
}