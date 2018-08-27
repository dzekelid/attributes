swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
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
      description: Lists all of the AWS DMS attributes for a customer account.
      operationId: describeAccountAttributes
      x-api-path-slug: actiondescribeaccountattributes-get
      parameters:
      - in: query
        name: AccountQuotas
        description: Account quota information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Attributes