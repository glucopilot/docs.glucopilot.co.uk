---
title: /api/v1/insulins/:id
position_number: 1.2
type: get
description: Get insulin
parameters:
  - name: id
    content: Insulin id
content_markdown: |-
  The insulin for the given id.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/insulins/3fa85f64-5717-4562-b3fc-2c963f66afa6 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "name": "string",
        "type": "Bolus",
        "duration": 0,
        "scale": 0,
        "peakTime": 0,
        "created": "2025-04-13T13:17:36.963Z"
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
