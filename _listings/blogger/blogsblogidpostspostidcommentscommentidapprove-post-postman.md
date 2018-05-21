{
  "info": {
    "name": "Blogger API Update Blog Post Comment",
    "_postman_id": "16030f0b-b0a0-4c50-a638-5bc42a3607b4",
    "description": "Marks a comment as not spam.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "comments",
      "item": [
        {
          "id": "16687247-5639-4232-aef0-587a97a39a77",
          "name": "blogger.comments.approve",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/posts/:postId/comments/:commentId/approve"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a comment as not spam"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e317d1ea-63d4-4bd4-911d-b0a20a485350"
            }
          ]
        }
      ]
    }
  ]
}