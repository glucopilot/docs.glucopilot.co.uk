---
title: /api/v1/readings
position_number: 1.1
type: post
description: Add reading
parameters:
  - name: created
    content: Date and time the reading was taken
  - name: glucoseLevel
    content: Glucose level in mg/dL
content_markdown: |-
  The reading will be added to your account.
  {: .success }

  Adds a manual glucose reading to your account.
left_code_blocks:
  - code_block: |-
      {
        "created": "2025-04-07T21:07:36.719Z",
        "glucoseLevel": 0
      }
    title: JSON
    language: json
right_code_blocks:
  - code_block: |2-
      "3fa85f64-5717-4562-b3fc-2c963f66afa6"
    title: 201 Created
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
---
