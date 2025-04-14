---
title: /api/v1/injections/:id
position_number: 1.2
type: get
description: Get injection
parameters:
  - name: id
    content: Injection id
content_markdown: |-
  The injection for the given id.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/injections/3fa85f64-5717-4562-b3fc-2c963f66afa6 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "created": "2025-04-14T17:11:03.360Z",
        "insulinId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "insulinName": "string",
        "units": 0
      }
    title: 200 OK
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
