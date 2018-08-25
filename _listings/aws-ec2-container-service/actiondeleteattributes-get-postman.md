{
  "info": {
    "name": "Amazon EC2 Container Service API Delete Attributes",
    "_postman_id": "f99e69b5-ce80-467e-9cff-7ce72ed7a128",
    "description": "Deletes one or more custom attributes from an Amazon ECS resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "e785007d-8466-411c-9b82-69e369af432b",
          "name": "createCluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateCluster?clusterName=clusterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon ECS cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d45c1f60-fc21-4d8a-bd37-56a8506dded7"
            }
          ]
        }
      ]
    },
    {
      "name": "Services",
      "item": [
        {
          "id": "05379bcc-d8a6-4ddc-a604-4cc7f788c26a",
          "name": "createService",
          "request": {
            "url": "http://example.com/api/?Action=CreateService?clientToken=clientToken&cluster=cluster&deploymentConfiguration=deploymentConfiguration&desiredCount=desiredCount&loadBalancers=loadBalancers&placementConstraints=placementConstraints&placementStrategy=placementStrategy&role=role&serviceName=serviceName&taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Runs and maintains a desired number of tasks from a specified task definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7baac84e-82cd-498d-bb8a-87d84cf03315"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes",
      "item": [
        {
          "id": "5bb5d9ad-f7e9-495c-aaa1-65194ca438da",
          "name": "deleteAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAttributes?attributes=attributes&cluster=cluster",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes one or more custom attributes from an Amazon ECS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6360993-1f4c-429f-bf1b-a84fd829864f"
            }
          ]
        }
      ]
    }
  ]
}