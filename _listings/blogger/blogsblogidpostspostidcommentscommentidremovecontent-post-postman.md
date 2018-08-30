{
  "info": {
    "name": "Blogger API Update Blog Post Comment",
    "_postman_id": "f1637770-291d-46cb-a0f4-8073c24c75ca",
    "description": "Removes the content of a comment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "comments",
      "item": [
        {
          "id": "685fdc4e-afdb-45d8-865f-91519d846c6c",
          "name": "blogger.comments.removeContent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/posts/:postId/comments/:commentId/removecontent"
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
            "description": "Removes the content of a comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f50e680-fb08-453a-918c-1145950c6a1a"
            }
          ]
        }
      ]
    }
  ]
}