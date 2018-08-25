---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Reset Network Interface Attribute
  version: 1.0.0
  description: Resets a network interface attribute.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAccountAttributes:
    get:
      summary: Describe Account Attributes
      description: Describes attributes of your AWS account.
      operationId: describeaccountattributes
      x-api-path-slug: actiondescribeaccountattributes-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensureidempotency
          of the request
        type: string
      - in: query
        name: Description
        description: A description for the new AMI in the destination region
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Encrypted
        description: Specifies whether the destination snapshots of the copied image
          should be encrypted
        type: string
      - in: query
        name: KmsKeyId
        description: The full ARN of the AWS Key Management Service (AWS KMS) CMK
          to use when encrypting the snapshots of an image during a copy operation
        type: string
      - in: query
        name: Name
        description: The name of the new AMI in the destination region
        type: string
      - in: query
        name: SourceImageId
        description: The ID of the AMI to copy
        type: string
      - in: query
        name: SourceRegion
        description: The name of the region that contains the AMI to copy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account
  /?Action=DescribeImageAttribute:
    get:
      summary: Describe Image Attribute
      description: Describes the specified attribute of the specified AMI.
      operationId: describeimageattribute
      x-api-path-slug: actiondescribeimageattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ExecutableBy.N
        description: Scopes the images by users with explicit launch permissions
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: ImageId.N
        description: One or more image IDs
        type: string
      - in: query
        name: Owner.N
        description: Filters the images by the owner
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Image
  /?Action=DescribeInstanceAttribute:
    get:
      summary: Describe Instance Attribute
      description: Describes the specified attribute of the specified instance.
      operationId: describeinstanceattribute
      x-api-path-slug: actiondescribeinstanceattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return in a single call
        type: string
      - in: query
        name: NextToken
        description: The token to request the next page of results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=DescribeNetworkInterfaceAttribute:
    get:
      summary: Describe Network Interface Attribute
      description: Describes a network interface attribute.
      operationId: describenetworkinterfaceattribute
      x-api-path-slug: actiondescribenetworkinterfaceattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: NetworkInterfaceId.N
        description: One or more network interface IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network Interface
  /?Action=DescribeSnapshotAttribute:
    get:
      summary: Describe Snapshot Attribute
      description: Describes the specified attribute of the specified snapshot.
      operationId: describesnapshotattribute
      x-api-path-slug: actiondescribesnapshotattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of snapshot results returned by DescribeSnapshots
          in      paginated output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeSnapshots
          request where MaxResults was used and the      results exceeded the value
          of that parameter
        type: string
      - in: query
        name: Owner.N
        description: Returns the snapshots owned by the specified owner
        type: string
      - in: query
        name: RestorableBy.N
        description: One or more AWS accounts IDs that can create volumes from the
          snapshot
        type: string
      - in: query
        name: SnapshotId.N
        description: One or more snapshot IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Drive Snapshot
  /?Action=DescribeVolumeAttribute:
    get:
      summary: Describe Volume Attribute
      description: Describes the specified attribute of the specified volume.
      operationId: describevolumeattribute
      x-api-path-slug: actiondescribevolumeattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of volume results returned by DescribeVolumes
          in paginated      output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeVolumes
          request where MaxResults was used and the results      exceeded the value
          of that parameter
        type: string
      - in: query
        name: VolumeId.N
        description: One or more volume IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volumes
  /?Action=DescribeVpcAttribute:
    get:
      summary: Describe Vpc Attribute
      description: Describes the specified attribute of the specified VPC.
      operationId: describevpcattribute
      x-api-path-slug: actiondescribevpcattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: VpcId.N
        description: One or more VPC IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC
  /?Action=ModifyImageAttribute:
    get:
      summary: Modify Image Attribute
      description: Modifies the specified attribute of the specified AMI.
      operationId: modifyimageattribute
      x-api-path-slug: actionmodifyimageattribute-get
      parameters:
      - in: query
        name: Architecture
        description: The architecture of the AMI
        type: string
      - in: query
        name: BlockDeviceMapping.N
        description: One or more block device mapping entries
        type: string
      - in: query
        name: Description
        description: A description for your AMI
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EnaSupport
        description: Set to true to enable enhanced networking with ENA for the AMI
          and any instances that you launch from the AMI
        type: string
      - in: query
        name: ImageLocation
        description: The full path to your AMI manifest in Amazon S3 storage
        type: string
      - in: query
        name: KernelId
        description: The ID of the kernel
        type: string
      - in: query
        name: Name
        description: A name for your AMI
        type: string
      - in: query
        name: RamdiskId
        description: The ID of the RAM disk
        type: string
      - in: query
        name: RootDeviceName
        description: The name of the root device (for example, /dev/sda1, or/dev/xvda)
        type: string
      - in: query
        name: SriovNetSupport
        description: Set to simple to enable enhanced networking with the Intel 82599
          Virtual Function interface for the AMI and any instances that you launch
          from the AMI
        type: string
      - in: query
        name: VirtualizationType
        description: The type of virtualization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Image
  /?Action=ModifyInstanceAttribute:
    get:
      summary: Modify Instance Attribute
      description: Modifies the specified attribute of the specified instance.
      operationId: modifyinstanceattribute
      x-api-path-slug: actionmodifyinstanceattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=ModifyNetworkInterfaceAttribute:
    get:
      summary: Modify Network Interface Attribute
      description: Modifies the specified network interface attribute.
      operationId: modifynetworkinterfaceattribute
      x-api-path-slug: actionmodifynetworkinterfaceattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: SourceDestCheck
        description: The source/destination checking attribute
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network Interface
  /?Action=ModifySnapshotAttribute:
    get:
      summary: Modify Snapshot Attribute
      description: Adds or removes permission settings for the specified snapshot.
      operationId: modifysnapshotattribute
      x-api-path-slug: actionmodifysnapshotattribute-get
      parameters:
      - in: query
        name: AutoEnableIO
        description: Indicates whether the volume should be auto-enabled for I/O operations
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshot
  /?Action=ModifySubnetAttribute:
    get:
      summary: Modify Subnet Attribute
      description: Modifies a subnet attribute.
      operationId: modifysubnetattribute
      x-api-path-slug: actionmodifysubnetattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ResourceId.N
        description: The IDs of one or more resources to tag
        type: string
      - in: query
        name: Tag.N
        description: One or more tags
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subnet
  /?Action=ModifyVolumeAttribute:
    get:
      summary: Modify Volume Attribute
      description: Modifies a volume attribute.
      operationId: modifyvolumeattribute
      x-api-path-slug: actionmodifyvolumeattribute-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Volume
  /?Action=ModifyVpcAttribute:
    get:
      summary: Modify Vpc Attribute
      description: Modifies the specified attribute of the specified VPC.
      operationId: modifyvpcattribute
      x-api-path-slug: actionmodifyvpcattribute-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DeliverLogsPermissionArn
        description: The ARN for the IAM role thats used to post flow logs to a CloudWatch
          Logs log group
        type: string
      - in: query
        name: LogGroupName
        description: The name of the CloudWatch log group
        type: string
      - in: query
        name: ResourceId.N
        description: One or more subnet, network interface, or VPC IDs
        type: string
      - in: query
        name: ResourceType
        description: The type of resource on which to create the flow log
        type: string
      - in: query
        name: TrafficType
        description: The type of traffic to log
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC
  /?Action=ResetImageAttribute:
    get:
      summary: Reset Image Attribute
      description: Resets an attribute of an AMI to its default value.
      operationId: resetimageattribute
      x-api-path-slug: actionresetimageattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ProductCode
        description: The product code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Image
  /?Action=ResetInstanceAttribute:
    get:
      summary: Reset Instance Attribute
      description: Resets an attribute of an instance to its default value.
      operationId: resetinstanceattribute
      x-api-path-slug: actionresetinstanceattribute-get
      parameters:
      - in: query
        name: AdditionalInfo
        description: Reserved
        type: string
      - in: query
        name: BlockDeviceMapping.N
        description: The block device mapping
        type: string
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the request
        type: string
      - in: query
        name: DisableApiTermination
        description: If you set this parameter to true, you cant terminate the instance            using
          the Amazon EC2 console, CLI, or API; otherwise, you can
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: EbsOptimized
        description: Indicates whether the instance is optimized for EBS I/O
        type: string
      - in: query
        name: IamInstanceProfile
        description: The IAM instance profile
        type: string
      - in: query
        name: ImageId
        description: The ID of the AMI, which you can get by calling DescribeImages
        type: string
      - in: query
        name: InstanceInitiatedShutdownBehavior
        description: Indicates whether an instance stops or terminates when you initiate
          shutdown from the instance (using the operating system command for system
          shutdown)
        type: string
      - in: query
        name: InstanceType
        description: The instance type
        type: string
      - in: query
        name: Ipv6Address.N
        description: '[EC2-VPC] Specify one or more IPv6 addresses from the range
          of the subnet to            associate with the primary network interface'
        type: string
      - in: query
        name: Ipv6AddressCount
        description: '[EC2-VPC] A number of IPv6 addresses to associate with the primary
          network            interface'
        type: string
      - in: query
        name: KernelId
        description: The ID of the kernel
        type: string
      - in: query
        name: KeyName
        description: The name of the key pair
        type: string
      - in: query
        name: MaxCount
        description: The maximum number of instances to launch
        type: string
      - in: query
        name: MinCount
        description: The minimum number of instances to launch
        type: string
      - in: query
        name: Monitoring
        description: The monitoring for the instance
        type: string
      - in: query
        name: NetworkInterface.N
        description: One or more network interfaces
        type: string
      - in: query
        name: Placement
        description: The placement for the instance
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary IPv4 address'
        type: string
      - in: query
        name: RamdiskId
        description: The ID of the RAM disk
        type: string
      - in: query
        name: SecurityGroup.N
        description: '[EC2-Classic, default VPC] One or more security group names'
        type: string
      - in: query
        name: SecurityGroupId.N
        description: One or more security group IDs
        type: string
      - in: query
        name: SubnetId
        description: '[EC2-VPC] The ID of the subnet to launch the instance into'
        type: string
      - in: query
        name: UserData
        description: The user data to make available to the instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Instance
  /?Action=ResetNetworkInterfaceAttribute:
    get:
      summary: Reset Network Interface Attribute
      description: Resets a network interface attribute.
      operationId: resetnetworkinterfaceattribute
      x-api-path-slug: actionresetnetworkinterfaceattribute-get
      parameters:
      - in: query
        name: Ipv6Addresses.N
        description: The IPv6 addresses to unassign from the network interface
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Network Interface
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---