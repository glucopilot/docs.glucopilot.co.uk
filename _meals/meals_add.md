---
title: /api/v1/meals
position_number: 5.1
type: post
description: Add meal
parameters:
  - name: name
    content: Meal name
  - name: mealIngredients
    content: Collection of meal ingredients
content_markdown: |-
  Adds the meal with the given name and ingredients.
left_code_blocks:
  - code_block: |-
      {
        "name": "string",
        "mealIngredients": [
          {
            "ingredient": {
              "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
              "userId": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
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
    title: JSON
    language: json
right_code_blocks:
  - code_block: |2-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
        "name": "string"
      }
    title: 201 Created
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
