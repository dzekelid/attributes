{
  "info": {
    "name": "Amazon RDS API Describe Account Attributes",
    "_postman_id": "0bad4f31-c6aa-42f1-8853-8509990acdf2",
    "description": "Lists all of the attributes for a customer account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Clusters",
      "item": [
        {
          "id": "2dba128c-25be-47fd-9dda-1f0830da0ac8",
          "name": "addroletodbcluster",
          "request": {
            "url": "http://example.com/api/?Action=AddRoleToDBCluster?DBClusterIdentifier=DBClusterIdentifier&RoleArn=RoleArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates an Identity and Access Management (IAM) role from an Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a86727c-2bee-4822-9dbe-4c63c8f1c33b"
            }
          ]
        },
        {
          "id": "f2aaed62-1594-40cd-9ca8-849434cf8e30",
          "name": "createdbcluster",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBCluster?AvailabilityZones.AvailabilityZone.N=AvailabilityZones.AvailabilityZone.N&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&DatabaseName=DatabaseName&DBClusterIdentifier=DBClusterIdentifier&DBClusterParameterGroupName=DBClusterParameterGroupName&DBSubnetGroupName=DBSubnetGroupName&Engine=Engine&EngineVersion=EngineVersion&KmsKeyId=KmsKeyId&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&ReplicationSourceIdentifier=ReplicationSourceIdentifier&StorageEncrypted=StorageEncrypted&Tags.Tag.N=Tags.Tag.N&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Aurora DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57d0ce10-0f68-4ca8-a163-3d42f2aec474"
            }
          ]
        },
        {
          "id": "4fa57ba5-57d5-42fc-9dcf-5e28269218aa",
          "name": "deletedbcluster",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBCluster?DBClusterIdentifier=DBClusterIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBCluster action deletes a previously provisioned DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "830b87fc-a641-49aa-a1c6-7d24ab12a72c"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "6503dc1c-f4ee-4134-a736-03f1f5a7b69d",
          "name": "addsourceidentifiertosubscription",
          "request": {
            "url": "http://example.com/api/?Action=AddSourceIdentifierToSubscription?SourceIdentifier=SourceIdentifier&SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a source identifier to an existing RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b5720f0-b3fc-4ef5-b6b3-f20fbd58352a"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "f57b1fd6-a216-4206-a32b-ffa983c9f614",
          "name": "addtagstoresource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceName=ResourceName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds metadata tags to an Amazon RDS resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2e090e8-56a8-44e9-b559-f25df075cfd6"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance Actions",
      "item": [
        {
          "id": "30bc8623-fe28-4910-83ae-d7fdb375086a",
          "name": "applypendingmaintenanceaction",
          "request": {
            "url": "http://example.com/api/?Action=ApplyPendingMaintenanceAction?ApplyAction=ApplyAction&OptInType=OptInType&ResourceIdentifier=ResourceIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a pending maintenance action to a resource (for example, to a DB instance)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "890bf473-22ff-4862-94d1-f6c4624ccc5a"
            }
          ]
        }
      ]
    },
    {
      "name": "Security Groups",
      "item": [
        {
          "id": "cdec3338-2676-4db6-8427-f4393c8036a4",
          "name": "authorizedbsecuritygroupingress",
          "request": {
            "url": "http://example.com/api/?Action=AuthorizeDBSecurityGroupIngress?CIDRIP=CIDRIP&DBSecurityGroupName=DBSecurityGroupName&EC2SecurityGroupId=EC2SecurityGroupId&EC2SecurityGroupName=EC2SecurityGroupName&EC2SecurityGroupOwnerId=EC2SecurityGroupOwnerId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables ingress to a DBSecurityGroup using one of two forms of authorization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64df7e87-5317-40f7-be9d-7abc9279d2e5"
            }
          ]
        },
        {
          "id": "046b014f-0e99-4ad2-8473-8489dde327b4",
          "name": "createdbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSecurityGroup?DBSecurityGroupDescription=DBSecurityGroupDescription&DBSecurityGroupName=DBSecurityGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d8569d3-0da8-41d6-b4ad-2bf7bc40e908"
            }
          ]
        },
        {
          "id": "7f440ad2-fda8-445f-9998-81a1d83a540f",
          "name": "deletedbsecuritygroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSecurityGroup?DBSecurityGroupName=DBSecurityGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB security group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93623b08-f0ce-4360-add6-eb878d60c9ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Parameter Groups",
      "item": [
        {
          "id": "3545f716-87af-43fd-9195-c237d2137b51",
          "name": "copydbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterParameterGroup?SourceDBClusterParameterGroupIdentifier=SourceDBClusterParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterParameterGroupDescription=TargetDBClusterParameterGroupDescription&TargetDBClusterParameterGroupIdentifier=TargetDBClusterParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86e4343f-3ada-45cc-8fa6-3a0a6cc7fdf8"
            }
          ]
        },
        {
          "id": "d14e5a73-a785-4ab0-9c70-eee4547e617f",
          "name": "createdbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName&DBParameterGroupFamily=DBParameterGroupFamily&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a595df2b-b1e3-4794-b01e-b66a574d5afa"
            }
          ]
        },
        {
          "id": "a4f3c3b6-8391-4564-9a73-c5162488fedf",
          "name": "deletedbclusterparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterParameterGroup?DBClusterParameterGroupName=DBClusterParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DB cluster parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac32bfe5-d8c6-4d25-9241-5024bc4aeca2"
            }
          ]
        }
      ]
    },
    {
      "name": "Cluster Snapshots",
      "item": [
        {
          "id": "6bc1c97a-c9eb-433b-b639-b1a7c62f0d92",
          "name": "copydbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBClusterSnapshot?SourceDBClusterSnapshotIdentifier=SourceDBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBClusterSnapshotIdentifier=TargetDBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8da1e184-a4c5-48c1-834c-912c4d0d5067"
            }
          ]
        },
        {
          "id": "8251b290-76c9-45f2-9ec7-b9a22702be1c",
          "name": "createdbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBClusterSnapshot?DBClusterIdentifier=DBClusterIdentifier&DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a DB cluster."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25d2dcb8-f5e1-4a64-b194-c32aa923533c"
            }
          ]
        },
        {
          "id": "9be37be2-f7e9-4d73-9304-10401ddd3770",
          "name": "deletedbclustersnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBClusterSnapshot?DBClusterSnapshotIdentifier=DBClusterSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB cluster snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe751e69-5199-4013-91fb-0b4c3e39e01e"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter Groups",
      "item": [
        {
          "id": "4a768a5a-5607-4f4d-9817-657acbd07eb1",
          "name": "copydbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBParameterGroup?SourceDBParameterGroupIdentifier=SourceDBParameterGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBParameterGroupDescription=TargetDBParameterGroupDescription&TargetDBParameterGroupIdentifier=TargetDBParameterGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cd390b4-3697-4722-adfd-7f5539c67b7a"
            }
          ]
        },
        {
          "id": "20cc5985-4be0-4ce7-a805-edb603a0e000",
          "name": "createdbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBParameterGroup?DBParameterGroupFamily=DBParameterGroupFamily&DBParameterGroupName=DBParameterGroupName&Description=Description&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB parameter group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15b52402-8650-4d89-844d-860be4c04b89"
            }
          ]
        },
        {
          "id": "e551cd61-9bed-43a1-a395-60e126ccf193",
          "name": "deletedbparametergroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBParameterGroup?DBParameterGroupName=DBParameterGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified DBParameterGroup."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63121bce-2bcb-4f10-8bfc-159275915467"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "08860e1f-ef82-44af-b94a-ff23dae30111",
          "name": "copydbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CopyDBSnapshot?CopyTags=CopyTags&KmsKeyId=KmsKeyId&PreSignedUrl=PreSignedUrl&SourceDBSnapshotIdentifier=SourceDBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N&TargetDBSnapshotIdentifier=TargetDBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified DB snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3dcb74fb-2585-4c8c-8137-2c7474c6d880"
            }
          ]
        },
        {
          "id": "a14751cc-bfe9-4f8a-a4ac-f2294bda1606",
          "name": "createdbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSnapshot?DBInstanceIdentifier=DBInstanceIdentifier&DBSnapshotIdentifier=DBSnapshotIdentifier&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b1a2a2f-dcc3-424e-aad5-72067c81057a"
            }
          ]
        },
        {
          "id": "13100641-6be5-4dd2-b687-3a1878cc3b72",
          "name": "deletedbsnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSnapshot?DBSnapshotIdentifier=DBSnapshotIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DBSnapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a815a09a-2959-4026-9da0-d55c72fac9e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Option Groups",
      "item": [
        {
          "id": "6aaa4d10-e846-4eb7-b95f-c34f14921124",
          "name": "copyoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CopyOptionGroup?SourceOptionGroupIdentifier=SourceOptionGroupIdentifier&Tags.Tag.N=Tags.Tag.N&TargetOptionGroupDescription=TargetOptionGroupDescription&TargetOptionGroupIdentifier=TargetOptionGroupIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Copies the specified option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "117fcc59-291c-4d4d-86f1-0ab59f2204b4"
            }
          ]
        },
        {
          "id": "b93c6db4-a6f9-4a44-bff1-a2296584197f",
          "name": "createoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateOptionGroup?EngineName=EngineName&MajorEngineVersion=MajorEngineVersion&OptionGroupDescription=OptionGroupDescription&OptionGroupName=OptionGroupName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0842fca4-509e-40e1-a76f-0bc8470f594c"
            }
          ]
        },
        {
          "id": "3b9d3b2c-d83d-4528-a48f-5b311fa3db05",
          "name": "deleteoptiongroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteOptionGroup?OptionGroupName=OptionGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing option group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a826ba9a-1dc7-4615-9f2c-0e7ef98777f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Instances",
      "item": [
        {
          "id": "c0bf486f-09ed-4650-a6e7-45e83573d4ba",
          "name": "createdbinstance",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstance?AllocatedStorage=AllocatedStorage&AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&BackupRetentionPeriod=BackupRetentionPeriod&CharacterSetName=CharacterSetName&CopyTagsToSnapshot=CopyTagsToSnapshot&DBClusterIdentifier=DBClusterIdentifier&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBName=DBName&DBParameterGroupName=DBParameterGroupName&DBSecurityGroups.DBSecurityGroupName.N=DBSecurityGroups.DBSecurityGroupName.N&DBSubnetGroupName=DBSubnetGroupName&Domain=Domain&DomainIAMRoleName=DomainIAMRoleName&Engine=Engine&EngineVersion=EngineVersion&Iops=Iops&KmsKeyId=KmsKeyId&LicenseModel=LicenseModel&MasterUsername=MasterUsername&MasterUserPassword=MasterUserPassword&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&MultiAZ=MultiAZ&OptionGroupName=OptionGroupName&Port=Port&PreferredBackupWindow=PreferredBackupWindow&PreferredMaintenanceWindow=PreferredMaintenanceWindow&PromotionTier=PromotionTier&PubliclyAccessible=PubliclyAccessible&StorageEncrypted=StorageEncrypted&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N&TdeCredentialArn=TdeCredentialArn&TdeCredentialPassword=TdeCredentialPassword&Timezone=Timezone&VpcSecurityGroupIds.VpcSecurityGroupId.N=VpcSecurityGroupIds.VpcSecurityGroupId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c15cf3b8-e4b4-4fde-b0f4-76695bf9a9ce"
            }
          ]
        },
        {
          "id": "284d6872-12c1-45a4-be4d-e3bf138e725c",
          "name": "createdbinstancereadreplica",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBInstanceReadReplica?AutoMinorVersionUpgrade=AutoMinorVersionUpgrade&AvailabilityZone=AvailabilityZone&CopyTagsToSnapshot=CopyTagsToSnapshot&DBInstanceClass=DBInstanceClass&DBInstanceIdentifier=DBInstanceIdentifier&DBSubnetGroupName=DBSubnetGroupName&Iops=Iops&MonitoringInterval=MonitoringInterval&MonitoringRoleArn=MonitoringRoleArn&OptionGroupName=OptionGroupName&Port=Port&PubliclyAccessible=PubliclyAccessible&SourceDBInstanceIdentifier=SourceDBInstanceIdentifier&StorageType=StorageType&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a DB instance for a DB instance running MySQL, MariaDB, or PostgreSQL that acts as a Read Replica of a source DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76aabc5b-01a2-4592-af55-cde6e95f24ca"
            }
          ]
        },
        {
          "id": "6fa8d359-b158-48d0-b663-64a5fdcc24e0",
          "name": "deletedbinstance",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBInstance?DBInstanceIdentifier=DBInstanceIdentifier&FinalDBSnapshotIdentifier=FinalDBSnapshotIdentifier&SkipFinalSnapshot=SkipFinalSnapshot",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The DeleteDBInstance action deletes a previously provisioned DB instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43e3c47b-6f0a-4a0e-944b-e2c2c5e6ddd4"
            }
          ]
        }
      ]
    },
    {
      "name": "Subnet Groups",
      "item": [
        {
          "id": "00fecde9-6c82-415c-a5f8-3e2b13372bf2",
          "name": "createdbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateDBSubnetGroup?DBSubnetGroupDescription=DBSubnetGroupDescription&DBSubnetGroupName=DBSubnetGroupName&SubnetIds.SubnetIdentifier.N=SubnetIds.SubnetIdentifier.N&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4cf6056e-e55c-45f6-86d0-dab70e0d5456"
            }
          ]
        },
        {
          "id": "0ac80766-65ab-43ce-aa8b-36150ea2f2da",
          "name": "deletedbsubnetgroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDBSubnetGroup?DBSubnetGroupName=DBSubnetGroupName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a DB subnet group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a181c659-1f92-4031-a251-3457156645a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Event Subscriptions",
      "item": [
        {
          "id": "66c71a6c-69bf-4d14-8ace-585224f76048",
          "name": "createeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=CreateEventSubscription?Enabled=Enabled&EventCategories.EventCategory.N=EventCategories.EventCategory.N&SnsTopicArn=SnsTopicArn&SourceIds.SourceId.N=SourceIds.SourceId.N&SourceType=SourceType&SubscriptionName=SubscriptionName&Tags.Tag.N=Tags.Tag.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce18e701-830b-401f-b9ab-5b1f149f1c94"
            }
          ]
        },
        {
          "id": "3ea2c0cf-340f-4546-9f31-aecfb8e5770b",
          "name": "deleteeventsubscription",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEventSubscription?SubscriptionName=SubscriptionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an RDS event notification subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8400d608-121d-42ab-8e30-babf738f6727"
            }
          ]
        }
      ]
    },
    {
      "name": "Accounts",
      "item": [
        {
          "id": "7c13f2a6-37f0-4a9a-81c8-ace1d54822ae",
          "name": "describeaccountattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountAttributes?AccountQuotas.AccountQuota.N=AccountQuotas.AccountQuota.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the attributes for a customer account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e08ed613-bddc-4dc0-9be0-e82bcab69d34"
            }
          ]
        }
      ]
    }
  ]
}