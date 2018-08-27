{
  "info": {
    "name": "AWS Simple Notification Service API Set Subscription Attributes",
    "_postman_id": "b4d8e24c-7142-485e-a58c-ae361dadbd7f",
    "description": "Allows a subscription owner to set an attribute of the topic to a new value.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Permissions",
      "item": [
        {
          "id": "94e79aab-1a52-4642-935c-4ee0b4692b8a",
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
              "id": "eb36477d-208d-4d69-aac9-1d9814216b1e"
            }
          ]
        },
        {
          "id": "090eaa7f-8e4a-4456-bda2-2abdb9707f5e",
          "name": "removePermission",
          "request": {
            "url": "http://example.com/api/?Action=RemovePermission?Label=Label&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a statement from a topic's access control policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26eecb17-0f1f-4d30-af85-41f82878a285"
            }
          ]
        }
      ]
    },
    {
      "name": "Opt Out",
      "item": [
        {
          "id": "6b1d280b-7734-40b5-9e12-2b408479cd4d",
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
              "id": "fa6aa2a1-753c-4e3e-a856-9363a035bdce"
            }
          ]
        },
        {
          "id": "e133c9db-6ce4-42d9-ac37-d6c2525951d9",
          "name": "listPhoneNumbersOptedOut",
          "request": {
            "url": "http://example.com/api/?Action=ListPhoneNumbersOptedOut?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of phone numbers that are opted out, meaning you cannot send SMS messages to them."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec67eb1e-23b6-4ec1-90d9-e72efc4cc2aa"
            }
          ]
        },
        {
          "id": "3e0794bc-af31-4ff3-a448-772bd4b20ea9",
          "name": "optInPhoneNumber",
          "request": {
            "url": "http://example.com/api/?Action=OptInPhoneNumber?phoneNumber=phoneNumber",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this request to opt in a phone number that is opted out, which enables you to resume sending SMS messages to the number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bc2b967-2643-4c22-883a-c6265c06f788"
            }
          ]
        }
      ]
    },
    {
      "name": "Subscriptions",
      "item": [
        {
          "id": "8cf1de95-e4ca-4666-b17f-a043662a2296",
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
              "id": "710da235-3d1d-4a16-b452-9bfbdd1b2c95"
            }
          ]
        },
        {
          "id": "ff5631f1-dd46-4bcd-ad15-dec501cce21f",
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
              "id": "9cc2ea6f-c1ea-4928-a5cf-4b95c8618a07"
            }
          ]
        },
        {
          "id": "cb53a164-02a9-43a4-baa5-487a420fae74",
          "name": "listSubscriptions",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptions?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's subscriptions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e64fea7-b755-4440-94b9-571844e31f81"
            }
          ]
        },
        {
          "id": "4d4f21d7-1aaf-4c83-bc26-3a33e3cefa28",
          "name": "listSubscriptionsByTopic",
          "request": {
            "url": "http://example.com/api/?Action=ListSubscriptionsByTopic?NextToken=NextToken&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the subscriptions to a specific topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc90ca16-fbd5-49e5-99a7-88b0ac3ee85c"
            }
          ]
        },
        {
          "id": "048efc76-f771-4969-98fb-c1b950aa9c71",
          "name": "setSubscriptionAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetSubscriptionAttributes?AttributeName=AttributeName&AttributeValue=AttributeValue&SubscriptionArn=SubscriptionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a subscription owner to set an attribute of the topic to a new value."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "223518bf-0c5b-466a-a9c6-43de58dd49d6"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Applications",
      "item": [
        {
          "id": "a89283a1-d67f-4659-ac02-f99f9f6a15fc",
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
              "id": "eebbac79-e8b2-4b54-9f2a-214b9121446c"
            }
          ]
        },
        {
          "id": "bd603a5e-e2c6-45bc-a44a-77235078c873",
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
              "id": "2bb2ffa8-166a-46f6-9615-dc151ac0c6a1"
            }
          ]
        },
        {
          "id": "beb95c32-9cfc-43a0-8215-3f631adea5c1",
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
              "id": "88f648c6-019b-4e3d-9789-72a2c6e2a42f"
            }
          ]
        },
        {
          "id": "e16cfbaf-7659-4361-ad74-17f569bb5494",
          "name": "listPlatformApplications",
          "request": {
            "url": "http://example.com/api/?Action=ListPlatformApplications?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the platform application objects for the supported push notification services, such as\n      APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74450561-fb57-4aca-a337-4ceff30dfc7a"
            }
          ]
        },
        {
          "id": "0536ac26-0549-497c-8c0a-8e7c22f77ebf",
          "name": "setPlatformApplicationAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetPlatformApplicationAttributes?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the attributes of the platform application object for the supported push notification\n      services, such as APNS and GCM."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcc5b98f-029d-479c-8ab1-8e076c43f754"
            }
          ]
        }
      ]
    },
    {
      "name": "Platform Endpoints",
      "item": [
        {
          "id": "00e66173-5269-4169-ace8-95bcf748a28a",
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
              "id": "46332b54-3b41-44c3-8886-258e291f4338"
            }
          ]
        }
      ]
    },
    {
      "name": "Topics",
      "item": [
        {
          "id": "465b56d3-0b59-43e0-9f03-4ebabd0ba8a4",
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
              "id": "93d41e09-47aa-413c-88a3-df219e6c241d"
            }
          ]
        },
        {
          "id": "bc000e5d-2e40-43f4-b766-4b14fee41976",
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
              "id": "80c87b80-0f05-4a41-a5ac-28075ca2d710"
            }
          ]
        },
        {
          "id": "94771ac2-13c4-4606-b962-c0606886398d",
          "name": "getTopicAttributes",
          "request": {
            "url": "http://example.com/api/?Action=GetTopicAttributes?TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all of the properties of a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "359e7e37-9bbc-4416-a79c-845c997bd610"
            }
          ]
        },
        {
          "id": "016f97ba-9579-4e26-99b6-0a61d2af1893",
          "name": "listTopics",
          "request": {
            "url": "http://example.com/api/?Action=ListTopics?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of the requester's topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7aff4206-ede4-4857-93b1-545e1c1f3b17"
            }
          ]
        }
      ]
    },
    {
      "name": "Endpoints",
      "item": [
        {
          "id": "72acab80-6a91-4636-aab5-56a1b82a82c8",
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
              "id": "78a63bbe-7a2a-4b42-be06-78a22a6d2c9d"
            }
          ]
        },
        {
          "id": "13553478-32a2-4426-9144-d8b94d0f96d0",
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
              "id": "01769c48-6001-447c-8702-ee5777b22591"
            }
          ]
        },
        {
          "id": "790e23da-a213-4c3e-af8d-51d1fedde974",
          "name": "listEndpointsByPlatformApplication",
          "request": {
            "url": "http://example.com/api/?Action=ListEndpointsByPlatformApplication?NextToken=NextToken&PlatformApplicationArn=PlatformApplicationArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the endpoints and endpoint attributes for devices in a supported push notification\n      service, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "237e6a55-1856-42db-accb-0b7575f99e11"
            }
          ]
        },
        {
          "id": "b1484318-1d0f-4ce0-a7cf-7a5a010ec578",
          "name": "setEndpointAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetEndpointAttributes?Attributes\n            , Attributes.entry.N.key (key), Attributesentry.N.value (value)=Attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20Attributes.entry.N.key%20%28key%29%2C%20Attributesentry.N.value%20%28value%29&EndpointArn=EndpointArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the attributes for an endpoint for a device on one of the supported push notification\n      services, such as GCM and APNS."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77d510a5-1125-44e4-904f-911f28e576ea"
            }
          ]
        }
      ]
    },
    {
      "name": "SMS",
      "item": [
        {
          "id": "445f1c99-1fcd-42ee-9b8b-a2ae1177c6f9",
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
              "id": "6e3b701b-66f8-40d2-a873-c5527e74e558"
            }
          ]
        },
        {
          "id": "52027519-ba85-4f3d-92a6-bd12132ce100",
          "name": "setSMSAttributes",
          "request": {
            "url": "http://example.com/api/?Action=SetSMSAttributes?attributes\n            , attributes.entry.N.key (key), attributesentry.N.value (value)=attributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20attributes.entry.N.key%20%28key%29%2C%20attributesentry.N.value%20%28value%29",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Use this request to set the default settings for sending SMS messages and receiving daily SMS usage reports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c3d1328-a665-4ff5-86fc-a14b899acde8"
            }
          ]
        }
      ]
    },
    {
      "name": "Publish",
      "item": [
        {
          "id": "336f87cd-8887-4d86-b2aa-2bfdafd85177",
          "name": "publish",
          "request": {
            "url": "http://example.com/api/?Action=Publish?Message=Message&MessageAttributes\n            , MessageAttributes.entry.N.Name (key), MessageAttributesentry.N.Value (value)=MessageAttributes%0A%20%20%20%20%20%20%20%20%20%20%20%20%2C%20MessageAttributes.entry.N.Name%20%28key%29%2C%20MessageAttributesentry.N.Value%20%28value%29&MessageStructure=MessageStructure&PhoneNumber=PhoneNumber&Subject=Subject&TargetArn=TargetArn&TopicArn=TopicArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message to all of a topic's subscribed endpoints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fe5dac3-ea59-4920-a263-7e13e5466af6"
            }
          ]
        }
      ]
    }
  ]
}