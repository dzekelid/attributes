---
swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 0
info:
  title: AWS Elastic Load Balancing API Modify Load Balancer Attributes
  version: 1.0.0
  description: Modifies the specified attributes of the specified Application Load
    Balancer.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeLoadBalancerAttributes:
    get:
      summary: Describe Load Balancer Attributes
      description: Describes the attributes for the specified Application Load Balancer.
      operationId: describeLoadBalancerAttributes
      x-api-path-slug: actiondescribeloadbalancerattributes-get
      parameters:
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=DescribeTargetGroupAttributes:
    get:
      summary: Describe Target Group Attributes
      description: Describes the attributes for the specified target group.
      operationId: describeTargetGroupAttributes
      x-api-path-slug: actiondescribetargetgroupattributes-get
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
  /?Action=ModifyLoadBalancerAttributes:
    get:
      summary: Modify Load Balancer Attributes
      description: Modifies the specified attributes of the specified Application
        Load Balancer.
      operationId: modifyLoadBalancerAttributes
      x-api-path-slug: actionmodifyloadbalancerattributes-get
      parameters:
      - in: query
        name: Attributes.member.N
        description: The load balancer attributes
        type: string
      - in: query
        name: LoadBalancerArn
        description: The Amazon Resource Name (ARN) of the load balancer
        type: string
      responses:
        200:
          description: OK
      tags:
      - Load Balancers
  /?Action=ModifyTargetGroupAttributes:
    get:
      summary: Modify Target Group Attributes
      description: Modifies the specified attributes of the specified target group.
      operationId: modifyTargetGroupAttributes
      x-api-path-slug: actionmodifytargetgroupattributes-get
      parameters:
      - in: query
        name: Attributes.member.N
        description: The attributes
        type: string
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      responses:
        200:
          description: OK
      tags:
      - Target Groups
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