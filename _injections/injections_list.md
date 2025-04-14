---
title: /api/v1/injections
position_number: 1.0
type: get
description: List injections
parameters:
  - name: page
    content: Page number to retrieve
  - name: pageSize
    content: Number of injections to retrieve per page
content_markdown: |-
  Injections are ordered by date descending.
  {: .info }

  Paginates all injections.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/injections?Page=1&PageSize=1 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "numberOfPages": 0,
        "injections": [
            {
            "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
            "created": "2025-04-13T21:51:38.532Z",
            "insulinId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
            "insulinName": "string",
            "units": 0
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
