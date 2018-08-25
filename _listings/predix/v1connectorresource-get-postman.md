{
  "info": {
    "name": "Predix Access Control Retrieves connector configuration for external resource attributes for the given zone.",
    "_postman_id": "a3d331b7-f071-47d6-bcab-559ef058f9b1",
    "description": "Retrieves connector configuration for external resource attributes for the given zone..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Monitoring",
      "item": [
        {
          "id": "2277e1e6-a18e-47b1-9339-d86d5568d2d1",
          "name": "getHeartBeatUsingGET",
          "request": {
            "url": "http://predix-acs.run.aws-usw02-pr.ice.predix.io/monitoring/heartbeat",
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
            "description": "Monitoring api that allows to check the acs heartbeat."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "32485724-3e94-406d-8263-0d90b6a8f0ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieves",
      "item": [
        {
          "id": "303c703e-abec-4aa2-9a41-28072f8f7160",
          "name": "getResourceConnectorUsingGET_1",
          "request": {
            "url": "http://predix-acs.run.aws-usw02-pr.ice.predix.io/v1/connector/resource",
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
            "description": "Retrieves connector configuration for external resource attributes for the given zone.."
          },
          "response": [
            {
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "9fb27aac-1c8f-4585-a34a-42d963f7347e"
            }
          ]
        }
      ]
    }
  ]
}