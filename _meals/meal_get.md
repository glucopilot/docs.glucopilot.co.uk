---
title: /api/v1/meals/:id
position_number: 1.2
type: get
description: Get meal
parameters:
  - name: id
    content: Meal id
content_markdown: |-
  The meal for the given id.
left_code_blocks:
  - code_block: |-
      curl http://api.myapp.com/api/v1/meals/3fa85f64-5717-4562-b3fc-2c963f66afa6 \
      -H "Authorization: Bearer YOUR_ACCESS_TOKEN"
    title: Curl
    language: bash
right_code_blocks:
  - code_block: |2-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "name": "string",
        "created": "2025-04-09T21:24:05.859Z",
        "mealIngredients": [
          {
            "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
            "ingredient": {
              "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
              "name": "string",
              "carbs": 0,
              "protein": 0,
              "fat": 0,
              "calories": 0,
              "uom": "Unit"
            },
            "quantity": 0
          }
        ]
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
