---
title: /api/v1/injections/:id
position_number: 1.4
type: delete
description: Remove injection
parameters:
  - name: id
    content: Injection id
left_code_blocks:
  - code_block: |-
      curl -X DELETE http://api.myapp.com/api/v1/injections/3fa85f64-5717-4562-b3fc-2c963f66afa6 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
    title: 204 NoContent
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
    title: 404 NotFound
    language: json
---
