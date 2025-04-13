---
title: /api/v1/insulins
position_number: 4.1
type: post
description: Add insulin
parameters:
content_markdown: |-
  Adds the insulin with the given name.
left_code_blocks:
  - code_block: |-
      {
        "name": "string",
        "type": "Bolus",
        "duration": 0,
        "scale": 0,
        "peakTime": 0
      }
    title: JSON
    language: json
right_code_blocks:
  - code_block: |2-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "name": "string",
        "type": "Bolus",
        "duration": 0,
        "scale": 0,
        "peakTime": 0,
        "created": "2025-04-13T09:21:35.406Z"
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
