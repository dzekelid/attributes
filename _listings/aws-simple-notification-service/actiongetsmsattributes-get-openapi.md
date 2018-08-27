---
swagger: "2.0"
x-collection-name: AWS Simple Notification Service
x-complete: 0
info:
  title: AWS Simple Notification Service API Get S M S Attributes
  version: 1.0.0
  description: Returns the settings for sending SMS messages from your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetEndpointAttributes:
    get:
      summary: Get Endpoint Attributes
      description: |-
        Retrieves the endpoint attributes for a device on one of the supported push notification
              services, such as GCM and APNS.
      operationId: getEndpointAttributes
      x-api-path-slug: actiongetendpointattributes-get
      parameters:
      - in: query
        name: EndpointArn
        description: EndpointArn for GetEndpointAttributes input
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=GetPlatformApplicationAttributes:
    get:
      summary: Get Platform Application Attributes
      description: |-
        Retrieves the attributes of the platform application object for the supported push
              notification services, such as APNS and GCM.
      operationId: getPlatformApplicationAttributes
      x-api-path-slug: actiongetplatformapplicationattributes-get
      parameters:
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for GetPlatformApplicationAttributesInput
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Applications
  /?Action=GetSMSAttributes:
    get:
      summary: Get S M S Attributes
      description: Returns the settings for sending SMS messages from your account.
      operationId: getSMSAttributes
      x-api-path-slug: actiongetsmsattributes-get
      parameters:
      - in: query
        name: attributes.member.N
        description: A list of the individual attribute names, such as MonthlySpendLimit,
          for which      you want values
        type: string
      responses:
        200:
          description: OK
      tags:
      - SMS
  /?Action=GetSubscriptionAttributes:
    get:
      summary: Get Subscription Attributes
      description: Returns all of the properties of a subscription.
      operationId: getSubscriptionAttributes
      x-api-path-slug: actiongetsubscriptionattributes-get
      parameters:
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=GetTopicAttributes:
    get:
      summary: Get Topic Attributes
      description: Returns all of the properties of a topic.
      operationId: getTopicAttributes
      x-api-path-slug: actiongettopicattributes-get
      parameters:
      - in: query
        name: TopicArn
        description: The ARN of the topic whose properties you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
  /?Action=SetEndpointAttributes:
    get:
      summary: Set Endpoint Attributes
      description: |-
        Sets the attributes for an endpoint for a device on one of the supported push notification
              services, such as GCM and APNS.
      operationId: setEndpointAttributes
      x-api-path-slug: actionsetendpointattributes-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: A map of the endpoint attributes
        type: string
      - in: query
        name: EndpointArn
        description: EndpointArn used for SetEndpointAttributes action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Endpoints
  /?Action=SetPlatformApplicationAttributes:
    get:
      summary: Set Platform Application Attributes
      description: |-
        Sets the attributes of the platform application object for the supported push notification
              services, such as APNS and GCM.
      operationId: setPlatformApplicationAttributes
      x-api-path-slug: actionsetplatformapplicationattributes-get
      parameters:
      - in: query
        name: |-
          Attributes
                      , Attributes.entry.N.key (key), Attributesentry.N.value (value)
        description: A map of the platform application attributes
        type: string
      - in: query
        name: PlatformApplicationArn
        description: PlatformApplicationArn for SetPlatformApplicationAttributes action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Platform Applications
  /?Action=SetSMSAttributes:
    get:
      summary: Set SMS Attributes
      description: Use this request to set the default settings for sending SMS messages
        and receiving daily SMS usage reports.
      operationId: setSMSAttributes
      x-api-path-slug: actionsetsmsattributes-get
      parameters:
      - in: query
        name: |-
          attributes
                      , attributes.entry.N.key (key), attributesentry.N.value (value)
        description: The default settings for sending SMS messages from your account
        type: string
      responses:
        200:
          description: OK
      tags:
      - SMS
  /?Action=SetSubscriptionAttributes:
    get:
      summary: Set Subscription Attributes
      description: Allows a subscription owner to set an attribute of the topic to
        a new value.
      operationId: setSubscriptionAttributes
      x-api-path-slug: actionsetsubscriptionattributes-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the attribute you want to set
        type: string
      - in: query
        name: AttributeValue
        description: The new value for the attribute in JSON format
        type: string
      - in: query
        name: SubscriptionArn
        description: The ARN of the subscription to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Subscriptions
  /?Action=SetTopicAttributes:
    get:
      summary: Set Topic Attributes
      description: Allows a topic owner to set an attribute of the topic to a new
        value.
      operationId: setTopicAttributes
      x-api-path-slug: actionsettopicattributes-get
      parameters:
      - in: query
        name: AttributeName
        description: The name of the attribute you want to set
        type: string
      - in: query
        name: AttributeValue
        description: The new value for the attribute
        type: string
      - in: query
        name: TopicArn
        description: The ARN of the topic to modify
        type: string
      responses:
        200:
          description: OK
      tags:
      - Topics
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