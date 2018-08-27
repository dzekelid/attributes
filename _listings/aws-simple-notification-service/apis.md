---
name: AWS Simple Notification Service
x-slug: aws-simple-notification-service
description: Amazon Simple Notification Service (Amazon SNS) is a fast, flexible,
  fully managed push notification service that lets you send individual messages or
  to fan-out messages to large numbers of recipients. Amazon SNS makes it simple and
  cost effective to send push notifications to mobile device users, email recipients
  or even send messages to other distributed services.With Amazon SNS, you can send
  notifications to Apple, Google, Fire OS, and Windows devices, as well as to Android
  devices in China with Baidu Cloud Push. You can use SNS to send SMS messages to
  mobile device users worldwide.Beyond these endpoints, Amazon SNS can also deliver
  messages toAmazon Simple Queue Service(SQS),AWS Lambda functions, or to any HTTP
  endpoint.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Attributes
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Simple Notification Service API - Get Endpoint Attributes
  x-api-slug: actiongetendpointattributes-get
  description: |-
    Retrieves the endpoint attributes for a device on one of the supported push notification
          services, such as GCM and APNS.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetendpointattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get Platform Application Attributes
  x-api-slug: actiongetplatformapplicationattributes-get
  description: |-
    Retrieves the attributes of the platform application object for the supported push
          notification services, such as APNS and GCM.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetplatformapplicationattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get S M S Attributes
  x-api-slug: actiongetsmsattributes-get
  description: Returns the settings for sending SMS messages from your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetsmsattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get Subscription Attributes
  x-api-slug: actiongetsubscriptionattributes-get
  description: Returns all of the properties of a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetsubscriptionattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetsubscriptionattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get Topic Attributes
  x-api-slug: actiongettopicattributes-get
  description: Returns all of the properties of a topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongettopicattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Endpoint Attributes
  x-api-slug: actionsetendpointattributes-get
  description: |-
    Sets the attributes for an endpoint for a device on one of the supported push notification
          services, such as GCM and APNS.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetendpointattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Platform Application Attributes
  x-api-slug: actionsetplatformapplicationattributes-get
  description: |-
    Sets the attributes of the platform application object for the supported push notification
          services, such as APNS and GCM.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetplatformapplicationattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set SMS Attributes
  x-api-slug: actionsetsmsattributes-get
  description: Use this request to set the default settings for sending SMS messages
    and receiving daily SMS usage reports.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetsmsattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Subscription Attributes
  x-api-slug: actionsetsubscriptionattributes-get
  description: Allows a subscription owner to set an attribute of the topic to a new
    value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetsubscriptionattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetsubscriptionattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Topic Attributes
  x-api-slug: actionsettopicattributes-get
  description: Allows a topic owner to set an attribute of the topic to a new value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsettopicattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get Endpoint Attributes
  x-api-slug: actiongetendpointattributes-get
  description: |-
    Retrieves the endpoint attributes for a device on one of the supported push notification
          services, such as GCM and APNS.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetendpointattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get Platform Application Attributes
  x-api-slug: actiongetplatformapplicationattributes-get
  description: |-
    Retrieves the attributes of the platform application object for the supported push
          notification services, such as APNS and GCM.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetplatformapplicationattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get S M S Attributes
  x-api-slug: actiongetsmsattributes-get
  description: Returns the settings for sending SMS messages from your account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetsmsattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get Subscription Attributes
  x-api-slug: actiongetsubscriptionattributes-get
  description: Returns all of the properties of a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetsubscriptionattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongetsubscriptionattributes-get-openapi.md
- name: AWS Simple Notification Service API - Get Topic Attributes
  x-api-slug: actiongettopicattributes-get
  description: Returns all of the properties of a topic.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actiongettopicattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Endpoint Attributes
  x-api-slug: actionsetendpointattributes-get
  description: |-
    Sets the attributes for an endpoint for a device on one of the supported push notification
          services, such as GCM and APNS.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetendpointattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Platform Application Attributes
  x-api-slug: actionsetplatformapplicationattributes-get
  description: |-
    Sets the attributes of the platform application object for the supported push notification
          services, such as APNS and GCM.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetplatformapplicationattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set SMS Attributes
  x-api-slug: actionsetsmsattributes-get
  description: Use this request to set the default settings for sending SMS messages
    and receiving daily SMS usage reports.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetsmsattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Subscription Attributes
  x-api-slug: actionsetsubscriptionattributes-get
  description: Allows a subscription owner to set an attribute of the topic to a new
    value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetsubscriptionattributes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsetsubscriptionattributes-get-openapi.md
- name: AWS Simple Notification Service API - Set Topic Attributes
  x-api-slug: actionsettopicattributes-get
  description: Allows a topic owner to set an attribute of the topic to a new value.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Mobile-Services_AmazonSNS.png
  humanURL: https://aws.amazon.com/sns/
  baseURL: :///
  tags: Amazon Web Services, Notifications, SMS, Stack Network, API Service Provider,
    API Service Provider, API Provider, Messages, Profiles, Relative Data, Service
    API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attributes/master/_listings/aws-simple-notification-service/actionsettopicattributes-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.simple.email.service.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.simple.notification.service.stack.network
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/Amazon-SN
- type: x-console
  url: https://console.aws.amazon.com/sns
- type: x-documentation
  url: http://docs.aws.amazon.com/sns/latest/api/
- type: x-faq
  url: https://aws.amazon.com/sns/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=72
- type: x-getting-started
  url: https://aws.amazon.com/sns/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/sns/pricing/
- type: x-website
  url: https://aws.amazon.com/sns/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---