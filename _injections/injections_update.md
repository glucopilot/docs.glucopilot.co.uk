---
title: /api/v1/injections/:id
position_number: 1.3
type: patch
description: Update injection
parameters:
  - name: id
    content: The id of the updated injection
content_markdown: |-
  The injection for the given id.
left_code_blocks:
  - code_block: |-
      {
        "insulinId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "units": 0,
        "type": "Bolus"
      }
    title: JSON
    language: json
right_code_blocks:
  - code_block: |-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "insulinId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "insulinName": "string",
        "units": 0
      }
    title: JSON
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
  - code_block: |2-
    title: 404 NotFound
    language: json
---
