---
title: /api/v1/meals
position_number: 1.0
type: get
description: List meals
parameters:
  - name: page
    content: Page number to retrieve
  - name: pageSize
    content: Number of meals to retrieve per page
content_markdown: |-
  Meals are ordered by date descending.
  {: .info }

  Paginates all meals.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/meals?page=0&pageSize=10 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "numberOfPages": 0,
        "meals": [
          {
            "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
            "name": "string",
            "created": "2025-04-07T23:07:22.802Z"
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
