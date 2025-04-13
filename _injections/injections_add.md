---
title: /api/v1/injections
position_number: 4.1
type: post
description: Add injection
parameters:
content_markdown: |-
  Adds the injection with the defined insulin and units.
left_code_blocks:
  - code_block: |-
      {
        "insulinId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "units": 0
      }
    title: JSON
    language: json
right_code_blocks:
  - code_block: |2-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "created": "2025-04-13T21:53:24.368Z",
        "insulinId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "units": 0
      }
    title: 200 Ok
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
