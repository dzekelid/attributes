{
  "info": {
    "name": "AWS EC2 API Describe Account Attributes",
    "_postman_id": "ac594202-a1af-45bb-bfc3-6d7ff07709e3",
    "description": "Describes attributes of your AWS account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "46522ed9-34a7-4568-8e71-13327628bb87",
          "name": "describeaccountattributes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountAttributes?ClientToken=ClientToken&Description=Description&DryRun=DryRun&Encrypted=Encrypted&KmsKeyId=KmsKeyId&Name=Name&SourceImageId=SourceImageId&SourceRegion=SourceRegion",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes attributes of your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70d09007-fd30-4e80-804b-f6220642cf4a"
            }
          ]
        }
      ]
    }
  ]
}