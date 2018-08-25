{
  "info": {
    "name": "Amazon EC2 Container Service API Put Attributes",
    "_postman_id": "b87b2c05-4f2b-4f8d-af63-1285b2f4086f",
    "description": "Create or update an attribute on an Amazon ECS resource.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "5eee56bc-2f76-4dde-b60a-50331582cdda",
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
              "id": "e7c87506-32ca-4d14-a56e-4b5682c6a03b"
            }
          ]
        },
        {
          "id": "740b5c6c-f04f-4054-b548-c04b5e37d857",
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
              "id": "bd39ade2-a396-442a-aedd-981a1837116e"
            }
          ]
        },
        {
          "id": "1cd44706-d8c5-4061-a73a-619c2f113540",
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
              "id": "2acd67b8-aae1-455d-a526-2f0c51ee2020"
            }
          ]
        },
        {
          "id": "71659ec2-45c6-4b06-b186-6cb3145d6237",
          "name": "listClusters",
          "request": {
            "url": "http://example.com/api/?Action=ListClusters?maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of existing clusters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a2f3221-0dae-42c1-93a7-3755e3bcbb8a"
            }
          ]
        }
      ]
    },
    {
      "name": "Services",
      "item": [
        {
          "id": "2676ebe1-fc74-4c94-9919-8431a286dae2",
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
              "id": "17e3f315-3807-497f-9f5b-af6f63489aa6"
            }
          ]
        },
        {
          "id": "b2ba5a78-58ec-4650-b4dd-d40362fe0d6f",
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
              "id": "ac565ae6-6a1c-4b42-8f8a-ae7ba3c65aaf"
            }
          ]
        },
        {
          "id": "6c010e2e-b1d2-4489-8ca8-436e8f80d90a",
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
              "id": "03253213-69b2-45ef-af90-d5666437c702"
            }
          ]
        },
        {
          "id": "55bb40e8-d495-4835-b1c4-404762d3590f",
          "name": "listServices",
          "request": {
            "url": "http://example.com/api/?Action=ListServices?cluster=cluster&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the services that are running in a specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4c1d164-e40d-4a3a-a1d9-5387d55ef93f"
            }
          ]
        }
      ]
    },
    {
      "name": "Attributes",
      "item": [
        {
          "id": "29fa921f-30f7-4a8e-8463-b3bbd32c05b8",
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
              "id": "50d61370-05a8-4c7d-8344-c7c0062b2480"
            }
          ]
        },
        {
          "id": "26d7b600-55e0-4caa-a5d9-52b512249c3a",
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
              "id": "b29af911-b553-4a15-a0ae-a1d7bd7a266a"
            }
          ]
        },
        {
          "id": "89eccf01-a073-4e70-ac5a-23811ccb4abf",
          "name": "putAttributes",
          "request": {
            "url": "http://example.com/api/?Action=PutAttributes?attributes=attributes&cluster=cluster",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create or update an attribute on an Amazon ECS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8d8d6b3-bb46-43f9-8e53-8189795ef2a1"
            }
          ]
        }
      ]
    },
    {
      "name": "Containers",
      "item": [
        {
          "id": "3bc902bf-1a9d-44e7-ad26-143576c570fa",
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
              "id": "4fe0abd4-ad0b-4780-afc1-7a2b812061d2"
            }
          ]
        },
        {
          "id": "baa160b2-89c0-46ae-b9e4-f6326818561c",
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
              "id": "07da6366-c0ac-426a-80ee-76aa619c6762"
            }
          ]
        },
        {
          "id": "34f9d7dc-d232-4b2d-a2c7-bdd6b8207d0c",
          "name": "listContainerInstances",
          "request": {
            "url": "http://example.com/api/?Action=ListContainerInstances?cluster=cluster&filter=filter&maxResults=maxResults&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of container instances in a specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d538c431-40e6-4bf6-bcb1-99794c30eeea"
            }
          ]
        }
      ]
    },
    {
      "name": "Task Definitions",
      "item": [
        {
          "id": "e1c220ff-232f-47ba-be44-1a1cb27be9a9",
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
              "id": "f67db559-42a5-49c3-a9fe-4e300763b2a3"
            }
          ]
        },
        {
          "id": "ba589dd2-3cc2-456e-be8c-36ce89fc2bac",
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
              "id": "ff9cba43-64bb-473a-88ab-31a01bedad3f"
            }
          ]
        },
        {
          "id": "7ad04aa7-5f4c-4ea5-96d0-5339ad1a5ac8",
          "name": "listTaskDefinitions",
          "request": {
            "url": "http://example.com/api/?Action=ListTaskDefinitions?familyPrefix=familyPrefix&maxResults=maxResults&nextToken=nextToken&sort=sort&status=status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of task definitions that are registered to your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b537586-3e73-43fa-a285-a0e6c7a5cbf0"
            }
          ]
        }
      ]
    },
    {
      "name": "Tasks",
      "item": [
        {
          "id": "eafcf1a9-d08e-491b-884a-689e15e68e9c",
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
              "id": "72e752dc-9ee2-4ea1-95bc-7dc86cc8749a"
            }
          ]
        },
        {
          "id": "2c699299-973a-49a8-a380-2660f1cb26f5",
          "name": "listTasks",
          "request": {
            "url": "http://example.com/api/?Action=ListTasks?cluster=cluster&containerInstance=containerInstance&desiredStatus=desiredStatus&family=family&maxResults=maxResults&nextToken=nextToken&serviceName=serviceName&startedBy=startedBy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of tasks for a specified cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00330944-b2bd-4988-8bcb-a01d13a27171"
            }
          ]
        }
      ]
    },
    {
      "name": "Poll Endpoints",
      "item": [
        {
          "id": "e9f25d08-da7d-4ad5-98b9-7f1076f5216c",
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
              "id": "10d4bea1-b239-4425-8e31-b9eb6c93e02d"
            }
          ]
        }
      ]
    },
    {
      "name": "Task Definition Families",
      "item": [
        {
          "id": "42986d7d-e935-4ebb-a74c-ff3f7f1581ec",
          "name": "listTaskDefinitionFamilies",
          "request": {
            "url": "http://example.com/api/?Action=ListTaskDefinitionFamilies?familyPrefix=familyPrefix&maxResults=maxResults&nextToken=nextToken&status=status",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of task definition families that are registered to your account\n            (which may include task definition families that no longer have any ACTIVE\n            task definition revisions)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c041951-d15f-4092-a8de-63e77dbbea6c"
            }
          ]
        }
      ]
    }
  ]
}