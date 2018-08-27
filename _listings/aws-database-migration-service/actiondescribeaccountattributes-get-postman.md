{
  "info": {
    "name": "AWS Database Migration Service API Describe Account Attributes",
    "_postman_id": "80486f18-e80c-4b25-a577-9b0b9aa56d00",
    "description": "Lists all of the AWS DMS attributes for a customer account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "f2921abd-9dae-4a53-9f63-5849d6b35e52",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceArn=ResourceArn&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds metadata tags to a DMS resource, including replication instance, endpoint, security group, and migration task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64b51acb-77b4-4ab3-929f-9604e5c3e58d"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "bbc8259e-ece6-4cd9-b94a-c0b9186aa46f",
          "name": "createEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=CreateEndpoint?CertificateArn=CertificateArn&DatabaseName=DatabaseName&EndpointIdentifier=EndpointIdentifier&EndpointType=EndpointType&EngineName=EngineName&ExtraConnectionAttributes=ExtraConnectionAttributes&KmsKeyId=KmsKeyId&Password=Password&Port=Port&ServerName=ServerName&SslMode=SslMode&Tags=Tags&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an endpoint using the provided settings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af502b24-fccd-46a9-9a77-9d23f28ae489"
            }
          ]
        },
        {
          "id": "e88911ea-fe2b-48ed-9cc0-408c47a8ab83",
          "name": "deleteEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEndpoint?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified endpoint."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb718ecf-a583-40b9-8ff9-896cdd30ef68"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Instances",
      "item": [
        {
          "id": "f5503094-4173-4778-b043-4fc546062e72",
          "name": "createReplicationInstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationInstance?AllocatedStorage=AllocatedStorage&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&EngineVersion=EngineVersion&KmsKeyId=KmsKeyId&MultiAZ=MultiAZ&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PubliclyAccessible=PubliclyAccessible&ReplicationInstanceClass=ReplicationInstanceClass&ReplicationInstanceIdentifier=ReplicationInstanceIdentifier&ReplicationSubnetGroupIdentifier=ReplicationSubnetGroupIdentifier&Tags=Tags&VpcSecurityGroupIds=VpcSecurityGroupIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the replication instance using the specified parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4283a241-4d2c-4755-aff3-36ed028a0b1f"
            }
          ]
        },
        {
          "id": "cd03a923-e0d5-4e63-bf36-bd6c4ad4b5af",
          "name": "deleteReplicationInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReplicationInstance?ReplicationInstanceArn=ReplicationInstanceArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified replication instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8329a33e-3305-4f6c-93a5-4d5e359d581d"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Subnet Group",
      "item": [
        {
          "id": "f00a5e2d-c92f-4334-8885-f2b47c90cc5a",
          "name": "createReplicationSubnetGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationSubnetGroup?ReplicationSubnetGroupDescription=ReplicationSubnetGroupDescription&ReplicationSubnetGroupIdentifier=ReplicationSubnetGroupIdentifier&SubnetIds=SubnetIds&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a replication subnet group given a list of the subnet IDs in a VPC."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9eade28-1d21-413f-8a3b-553aa7ef1bcb"
            }
          ]
        },
        {
          "id": "f40eb99b-3948-4e2d-a06a-a5baea1fb8b2",
          "name": "deleteReplicationSubnetGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReplicationSubnetGroup?ReplicationSubnetGroupIdentifier=ReplicationSubnetGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "506f8135-90e6-4c10-ab6a-dfa0ae20bb6d"
            }
          ]
        }
      ]
    },
    {
      "name": "Replication Tasks",
      "item": [
        {
          "id": "ffeb8fb7-bc73-42aa-8c84-4b728849a2d6",
          "name": "createReplicationTask",
          "request": {
            "url": "http://example.com/api/?Action=CreateReplicationTask?CdcStartTime=CdcStartTime&MigrationType=MigrationType&ReplicationInstanceArn=ReplicationInstanceArn&ReplicationTaskIdentifier=ReplicationTaskIdentifier&ReplicationTaskSettings=ReplicationTaskSettings&SourceEndpointArn=SourceEndpointArn&TableMappings=TableMappings&Tags=Tags&TargetEndpointArn=TargetEndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a replication task using the specified parameters."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b263ddb2-2d38-42d6-8fcc-2498fce89c73"
            }
          ]
        },
        {
          "id": "71d64f72-a75d-4b96-b280-769b18641c48",
          "name": "deleteReplicationTask",
          "request": {
            "url": "http://example.com/api/?Action=DeleteReplicationTask?ReplicationTaskArn=ReplicationTaskArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified replication task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88728f7b-c75e-4d17-b6a3-8e68dfb845a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "e22c4fd5-c990-4b0d-9613-e0ff9fcef8da",
          "name": "deleteCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCertificate?CertificateArn=CertificateArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7e2bbcc-aedc-4443-866a-0f8aea26c787"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Attributes",
      "item": [
        {
          "id": "90be74eb-96ba-49da-8ba2-746ac89e86f4",
          "name": "describeAccountAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountAttributes?AccountQuotas=AccountQuotas",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the AWS DMS attributes for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5478fb3c-a2b7-42e9-aad8-4590eae8cfc7"
            }
          ]
        }
      ]
    }
  ]
}