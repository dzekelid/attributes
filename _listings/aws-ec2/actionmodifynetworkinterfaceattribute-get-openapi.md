---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Modify Network Interface Attribute
  version: 1.0.0
  description: Modifies the specified network interface attribute.
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