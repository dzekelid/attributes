---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddCustomAttributes:
    get:
      summary: Add Custom Attributes
      description: Adds additional user attributes to the user pool schema.
      operationId: addCustomAttributes
      x-api-path-slug: actionaddcustomattributes-get
      parameters:
      - in: query
        name: CustomAttributes
        description: An array of custom attributes, such as Mutable and Name
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to add custom            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Attributes
  /?Action=AdminDeleteUserAttributes:
    get:
      summary: Admin Delete User Attributes
      description: Deletes the user attributes in a user pool as an administrator.
      operationId: adminDeleteUserAttributes
      x-api-path-slug: actionadmindeleteuserattributes-get
      parameters:
      - in: query
        name: UserAttributeNames
        description: An array of strings representing the user attribute names you
          wish to            delete
        type: string
      - in: query
        name: Username
        description: The user name of the user from which you would like to delete
          attributes
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to delete user            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=AdminUpdateUserAttributes:
    get:
      summary: Admin Update User Attributes
      description: |-
        Updates the specified user's attributes, including developer attributes, as an
                    administrator.
      operationId: adminUpdateUserAttributes
      x-api-path-slug: actionadminupdateuserattributes-get
      parameters:
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      - in: query
        name: Username
        description: The user name of the user for whom you want to update user attributes
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to update user            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=DeleteUserAttributes:
    get:
      summary: Delete User Attributes
      description: Deletes the attributes for a user.
      operationId: deleteUserAttributes
      x-api-path-slug: actiondeleteuserattributes-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token used in the request to delete user attributes
        type: string
      - in: query
        name: UserAttributeNames
        description: An array of strings representing the user attribute names you
          wish to            delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=UpdateUserAttributes:
    get:
      summary: Update User Attributes
      description: Allows a user to update a specific attribute (one at a time).
      operationId: updateUserAttributes
      x-api-path-slug: actionupdateuserattributes-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token for the request to update user attributes
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
  /?Action=GetUserAttributeVerificationCode:
    get:
      summary: Get User Attribute Verification Code
      description: |-
        Gets the user attribute verification code for the specified attribute
                    name.
      operationId: getUserAttributeVerificationCode
      x-api-path-slug: actiongetuserattributeverificationcode-get
      parameters:
      - in: query
        name: AccessToken
        description: The access token returned by the server response to get the user
          attribute            verification code
        type: string
      - in: query
        name: AttributeName
        description: The attribute name returned by the server response to get the
          user attribute            verification code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Verification Codes
  /?Action=VerifyUserAttribute:
    get:
      summary: Verify User Attribute
      description: Verifies the specified user attributes in the user pool.
      operationId: verifyUserAttribute
      x-api-path-slug: actionverifyuserattribute-get
      parameters:
      - in: query
        name: AccessToken
        description: Represents the access token of the request to verify user attributes
        type: string
      - in: query
        name: AttributeName
        description: The attribute name in the request to verify user attributes
        type: string
      - in: query
        name: Code
        description: The verification code in the request to verify user attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - Users
---