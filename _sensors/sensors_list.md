---
title: /api/v1/sensors
position_number: 1.0
type: get
description: List sensors
parameters:
  - name: page
    content: Page number to retrieve
  - name: pageSize
    content: Number of sensors to retrieve per page
content_markdown: |-
  Sensors are ordered by date descending.
  {: .info }

  Paginates all sensors.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/sensors?Page=0&PageSize=10 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "numberOfPages": 0,
        "sensors": [
            {
            "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
            "sensorId": "string",
            "started": "2025-04-17T13:29:21.120Z",
            "expires": "2025-04-17T13:29:21.120Z"
            }
        ]
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
