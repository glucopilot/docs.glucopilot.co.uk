---
title: /api/v1/identity/verify-email
position_number: 1.2
type: post
description: Verifies a user's email address
parameters:
  - name: token
    content: The verification token sent to the user's email address
content_markdown: |-
  The user's email address is verified using the provided token.
  {: .success}

  Verifies a user's email address using the provided token.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/identity/verify-email?token=string
    title: Curl
    language: curl
right_code_blocks:
  - code_block: |-
      <h1>Success</h1>
      <p>Your email has been verified.</p>
    title: 200 OK
    language: html
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
---
