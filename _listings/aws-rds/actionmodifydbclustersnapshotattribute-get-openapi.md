---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 0
info:
  title: Amazon RDS API Modify D B Cluster Snapshot Attribute
  version: 1.0.0
  description: Adds an attribute and values to, or removes an attribute and values
    from, a manual DB cluster snapshot.
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
      description: Lists all of the attributes for a customer account.
      operationId: describeaccountattributes
      x-api-path-slug: actiondescribeaccountattributes-get
      parameters:
      - in: query
        name: AccountQuotas.AccountQuota.N
        description: A list of AccountQuota objects
        type: string
      responses:
        200:
          description: OK
      tags:
      - Accounts
  /?Action=DescribeDBClusterSnapshotAttributes:
    get:
      summary: Describe D B Cluster Snapshot Attributes
      description: Returns a list of DB cluster snapshot attribute names and values
        for a manual DB cluster snapshot.
      operationId: describedbclustersnapshotattributes
      x-api-path-slug: actiondescribedbclustersnapshotattributes-get
      parameters:
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to describe the attributes
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
  /?Action=DescribeDBSnapshotAttributes:
    get:
      summary: Describe D B Snapshot Attributes
      description: Returns a list of DB snapshot attribute names and values for a
        manual DB snapshot.
      operationId: describedbsnapshotattributes
      x-api-path-slug: actiondescribedbsnapshotattributes-get
      parameters:
      - in: query
        name: DBSnapshotIdentifier
        description: The identifier for the DB snapshot to describe the attributes
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=ModifyDBClusterSnapshotAttribute:
    get:
      summary: Modify D B Cluster Snapshot Attribute
      description: Adds an attribute and values to, or removes an attribute and values
        from, a manual DB cluster snapshot.
      operationId: modifydbclustersnapshotattribute
      x-api-path-slug: actionmodifydbclustersnapshotattribute-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the DB cluster snapshot attribute to modify
        type: string
      - in: query
        name: DBClusterSnapshotIdentifier
        description: The identifier for the DB cluster snapshot to modify the attributes
          for
        type: string
      - in: query
        name: ValuesToAdd.AttributeValue.N
        description: A list of DB cluster snapshot attributes to add to the attribute
          specified by AttributeName
        type: string
      - in: query
        name: ValuesToRemove.AttributeValue.N
        description: A list of DB cluster snapshot attributes to remove from the attribute
          specified by AttributeName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Snapshots
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