{
  "info": {
    "name": "AWS Simple Notification Service API Get Subscription Attributes",
    "_postman_id": "06da6b38-b40a-4f5b-aeec-278456a8b2fa",
    "description": "Returns all of the properties of a subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "69834396-fe3c-418a-b107-9c2b1f2baf15",
          "name": "addPermission",
          "request": {
            "url": "http://example.com/api/?Action=AddPermission?ActionName.member.N=ActionName.member.N&AWSAccountId.member.N=AWSAccountId.member.N&Label=Label&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a statement to a topic's access control policy, granting access for the specified AWS accounts to the specified actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a8ff5ab-f9bf-4a89-9beb-90e9e4a71898"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "43441a47-8654-4069-a74c-7c2822fa6dd4",
          "name": "checkIfPhoneNumberIsOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=CheckIfPhoneNumberIsOptedOut?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a phone number and indicates whether the phone holder has opted out of receiving SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19c4bdf5-c24b-4d7a-bd26-f0fac8ce1189"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "d4f972df-18b2-451f-8d5e-dfc0311f3d26",
          "name": "confirmSubscription",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSubscription?AuthenticateOnUnsubscribe=AuthenticateOnUnsubscribe&Token=Token&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies an endpoint owner's intent to receive messages by validating the token sent to the\n      endpoint by an earlier Subscribe action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bade1701-a91c-4d14-9bb8-ba2a97c25c42"
            }
          ]
        },
        {
          "id": "6d10c805-8a6a-4941-a443-01f8bb1b1387",
          "name": "getSubscriptionAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSubscriptionAttributes?SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ed5dec8-584f-4945-b026-d75a05d964a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Applications",
      "item": [
        {
          "id": "0bf7b1be-2350-4a4e-8e82-88b6d9a5175f",
          "name": "createPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformApplication?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&Name=Name&Platform=Platform",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a platform application object for one of the supported push notification services,\n      such as APNS and GCM, to which devices and mobile apps may register."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fb605bd-4b73-4efd-bb1d-fc6e0c326739"
            }
          ]
        },
        {
          "id": "f040f666-7c7b-4f94-8492-27246d6cd02c",
          "name": "deletePlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=DeletePlatformApplication?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a platform application object for one of the supported push notification services,\n      such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31c1f385-6e01-4482-8055-1270e6b1fcea"
            }
          ]
        },
        {
          "id": "bc50e2ea-6486-4b18-ba48-2e8399b66a05",
          "name": "getPlatformApplicationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetPlatformApplicationAttributes?PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the attributes of the platform application object for the supported push\n      notification services, such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d2f2da3-8335-4528-8167-46f37b2f059d"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Endpoints",
      "item": [
        {
          "id": "5e12abb6-01dc-42cc-9195-45b1f3f3d828",
          "name": "createPlatformEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=CreatePlatformEndpoint?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&CustomUserData=CustomUserData&PlatformApplicationArn=PlatformApplicationArn&Token=Token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an endpoint for a device and mobile app on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e2570bb-a8a8-4bb7-a1ba-b771037718e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Topics",
      "item": [
        {
          "id": "1ef96e96-f4f5-4a9d-ae22-ea51f323e2f2",
          "name": "createTopic",
          "request": {
            "url": "http://example.com/api/?Action=CreateTopic?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a topic to which notifications can be published."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62756591-522a-4224-8a5b-fd92adf08f75"
            }
          ]
        },
        {
          "id": "9884774f-b114-4e48-8d95-b1b21672fed9",
          "name": "deleteTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTopic?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a topic and all its subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f6bdb28-d703-44e2-98d4-246ad8bbf4b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "a6ffa0be-396f-44c4-bd69-f94224109a5e",
          "name": "deleteEndpoint",
          "request": {
            "url": "http://example.com/api/?Action=DeleteEndpoint?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the endpoint for a device and mobile app from Amazon SNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5c9c717-0f33-46d3-978c-9bc95ea9e89b"
            }
          ]
        },
        {
          "id": "7addbae8-0ca2-4a53-869b-21de367875eb",
          "name": "getEndpointAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetEndpointAttributes?EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the endpoint attributes for a device on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "775af3ef-4d49-4b19-be1a-6770607af514"
            }
          ]
        }
      ]
    },
    {
      "name": "SMS",
      "item": [
        {
          "id": "46b79057-c120-4c06-ab80-f6b184d8421e",
          "name": "getSMSAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetSMSAttributes?attributes.member.N=attributes.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the settings for sending SMS messages from your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9ce2c34-ca99-49b9-bc23-1a963463ed65"
            }
          ]
        }
      ]
    }
  ]
}