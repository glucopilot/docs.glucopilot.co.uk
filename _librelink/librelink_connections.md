---
title: /api/v1/librelink/connections
position_number: 1.1
type: get
description: List connections
parameters:
content_markdown: |-
  Lists all the users LibreLink connections.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/librelink/connections \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      [
        {
          "patientId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
          "firstName": "string",
          "lastName": "string"
        }
      ]
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
---
