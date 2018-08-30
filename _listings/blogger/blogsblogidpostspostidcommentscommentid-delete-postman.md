{
  "info": {
    "name": "Blogger API Delete Blog Post Comments",
    "_postman_id": "f725221e-3a4e-44e5-a83e-f864b8b933d2",
    "description": "Delete a comment by ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "comments",
      "item": [
        {
          "id": "939f7440-039d-4def-861f-3d4912f2eeed",
          "name": "blogger.comments.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/posts/:postId/comments/:commentId"
              ],
              "variable": [
                {
                  "id": "blogId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "commentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "postId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a comment by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a4be753-5f44-45b8-8c6f-cf7aa6e45d60"
            }
          ]
        }
      ]
    }
  ]
}