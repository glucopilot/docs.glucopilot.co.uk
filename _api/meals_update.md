---
title: /api/v1/meals/:id
position_number: 1.2
type: patch
description: Update meal
parameters:
  - name: id
    content: The id of the updated meal
content_markdown: |-
  The meal for the given id.
left_code_blocks:
  - code_block: |-
      {
        "id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
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
    title: 204 NoContent
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
  - code_block: |2-
    title: 404 NotFound
    language: json
---
