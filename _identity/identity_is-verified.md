---
title: /api/v1/identity/is-verified
position_number: 1.3
type: get
description: Determines whether a user is email verified
parameters:
  - name: token
    content: The verification token sent to the user's email address
content_markdown: |-
  HTTP204 NoContent: The user's email has been verified.
  {: .success}

  HTTP403 Forbidden: The user's email has not been verified.
  {: .error}

  Indicates whether or not the requested user is email verified or not.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/identity/is-verified?email=string
    title: Curl
    language: curl
right_code_blocks:
  - code_block: |-
    title: 204 NoContent
    language: json
  - code_block: |-
      {
        "type": "string",
        "title": "string",
        "status": 0,
        "detail": "string",
        "instance": "string",
        "errors": {
          "additionalProp1": [
            "string"
          ],
          "additionalProp2": [
            "string"
          ],
          "additionalProp3": [
            "string"
          ]
        },
        "additionalProp1": "string",
        "additionalProp2": "string",
        "additionalProp3": "string"
      }
    title: 400 BadRequest
    language: json
  - code_block: |2-
      {
        "source": "string",
        "message": "string",
        "errorId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "supportMessage": "string",
        "statusCode": 0,
        "messages": [
          "string"
        ]
      }
    title: 401 Unauthorized
    language: json
  - code_block: |-
      {
        "source": "string",
        "message": "string",
        "errorId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "supportMessage": "string",
        "statusCode": 0,
        "messages": [
          "string"
        ]
      }
    title: 403 Forbidden
    language: json
---
