{
  "info": {
    "name": "Amazon EC2 Container Service API List Attributes",
    "_postman_id": "94b3bd1d-b7d0-417e-8ba6-956101b66980",
    "description": "Lists the attributes for Amazon ECS resources within a specified target type and\n            cluster.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "665aa045-18d2-42a1-9221-faea376555c6",
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
              "id": "53aca883-a817-46e6-9ff9-05cba29878eb"
            }
          ]
        },
        {
          "id": "b5caadd1-7337-489a-8481-2c597eebd954",
          "name": "deleteCluster",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCluster?cluster=cluster",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2563ae29-f2f7-4519-a737-021746ffdf41"
            }
          ]
        },
        {
          "id": "2cb28565-90fa-40e3-803a-81ca42e26dd6",
          "name": "describeClusters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeClusters?clusters=clusters",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your clusters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bff834d-3245-4125-a138-ff44f8671ac4"
            }
          ]
        }
      ]
    },
    {
      "name": "Services",
      "item": [
        {
          "id": "83a2c9d5-9eee-4c0a-8e19-c9020ce43d62",
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
              "id": "d1aea381-3f52-4ed6-ae6d-0ee957964729"
            }
          ]
        },
        {
          "id": "4b949b37-0f3f-4224-9042-b35d7c0589d7",
          "name": "deleteService",
          "request": {
            "url": "http://example.com/api/?Action=DeleteService?cluster=cluster&service=service",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified service within a cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "169a9f9f-7f0c-41dd-aec5-3b7b1243130a"
            }
          ]
        },
        {
          "id": "2cd1ad51-cc69-477e-a3e4-1c3397de992d",
          "name": "describeServices",
          "request": {
            "url": "http://example.com/api/?Action=DescribeServices?cluster=cluster&services=services",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified services running in your cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08adfb8f-fb56-40b1-85d7-17e28ab0366c"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes",
      "item": [
        {
          "id": "307cdcb9-4abc-4234-8175-8a9d39f5d048",
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
              "id": "216e2613-0fb8-477e-9af9-672b771f3d13"
            }
          ]
        },
        {
          "id": "0b4cb9ad-9b51-461d-ad76-a23c6fbd7563",
          "name": "listAttributes",
          "request": {
            "url": "http://example.com/api/?Action=ListAttributes?attributeName=attributeName&attributeValue=attributeValue&cluster=cluster&maxResults=maxResults&nextToken=nextToken&targetType=targetType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the attributes for Amazon ECS resources within a specified target type and\n            cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7af8db5-2391-47d2-9d40-e1ea92f574bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Containers",
      "item": [
        {
          "id": "ea072fa5-d13b-4cee-845f-7ea7d979cbe8",
          "name": "deregisterContainerInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterContainerInstance?cluster=cluster&containerInstance=containerInstance&force=force",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters an Amazon ECS container instance from the specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e50476f0-5e88-464d-ae0a-a35ff1df31ba"
            }
          ]
        },
        {
          "id": "fe29ed59-2213-447c-b157-08cf29de8af4",
          "name": "describeContainerInstances",
          "request": {
            "url": "http://example.com/api/?Action=DescribeContainerInstances?cluster=cluster&containerInstances=containerInstances",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes Amazon EC2 Container Service container instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34689fd3-eefa-4136-9992-31837367ebbf"
            }
          ]
        }
      ]
    },
    {
      "name": "Task Definitions",
      "item": [
        {
          "id": "bb0b28c2-bbd0-4131-ad5e-e00566115ec1",
          "name": "deregisterTaskDefinition",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskDefinition?taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deregisters the specified task definition by family and revision."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ecba52f-4ec2-4e16-a515-0829366795f9"
            }
          ]
        },
        {
          "id": "87555f16-a044-417c-bda5-09d05454c254",
          "name": "describeTaskDefinition",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTaskDefinition?taskDefinition=taskDefinition",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a task definition."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ccccfe59-ede5-42a7-8952-6ef107cbd3be"
            }
          ]
        }
      ]
    },
    {
      "name": "Tasks",
      "item": [
        {
          "id": "566a168a-6ca5-456f-904b-c1b19a34b8fd",
          "name": "describeTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTasks?cluster=cluster&tasks=tasks",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes a specified task or tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a7e2aef-9236-4747-b484-78327625ad3f"
            }
          ]
        }
      ]
    },
    {
      "name": "Poll Endpoints",
      "item": [
        {
          "id": "310568cc-fd28-46e9-b068-24ca433bbaa5",
          "name": "discoverPollEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DiscoverPollEndpoint",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This action is only used by the Amazon EC2 Container Service agent, and it is not intended for use outside of the agent."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72f89e66-e321-4bbc-a49f-c7094245ed2e"
            }
          ]
        }
      ]
    }
  ]
}