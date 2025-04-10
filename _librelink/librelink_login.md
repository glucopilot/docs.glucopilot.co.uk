---
title: /api/v1/librelink/login
position_number: 1.0
type: post
description: LibreLink Authenticate
parameters:
  - name: username
    content: The username of the LibreLink Up user
  - name: password
    content: The password of the LibreLink Up user
content_markdown: |-
  Authenticates GlucoPilot patient with LibreLink Up.
left_code_blocks:
  - code_block: |-
      {
        "username": "string",
        "password": "string"
      }
    title: JSON
    language: json
right_code_blocks:
  - code_block: |2-
      {
        "token": "string",
        "expires": 0,
        "duration": 0
      }
    title: 200 OK
    language: json
  - code_block: |2-
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
    title: 400 Bad Request
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
