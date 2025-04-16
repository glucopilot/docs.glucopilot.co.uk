---
title: /api/v1/treatments
position_number: 1.4
type: get
description: List treatments
parameters:
  - name: page
    content: Page number to retrieve
  - name: pageSize
    content: Number of treatments to retrieve per page
content_markdown: |-
  Treatments are ordered by date descending.
  {: .info }

  Paginates all treatments.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/treatments?Page=0&PageSize=10 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "numberOfPages": 0,
        "treatments": [
            {
            "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
            "created": "2025-04-16T21:07:08.073Z",
            "type": "Meal",
            "meal": {
                "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
                "name": "string",
                "totalCarbs": 0,
                "totalProtein": 0,
                "totalFat": 0,
                "totalCalories": 0
            },
            "injection": {
                "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
                "insulinName": "string",
                "units": 0
            },
            "reading": {
                "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
                "glucoseLevel": 0
            }
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
