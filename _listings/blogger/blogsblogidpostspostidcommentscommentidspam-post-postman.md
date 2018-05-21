{
  "info": {
    "name": "Blogger API Update Blog Post Comment SPAM",
    "_postman_id": "f85ce2ab-8621-404c-9e0b-3cd9eeb80ef0",
    "description": "Marks a comment as spam.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "comments",
      "item": [
        {
          "id": "c829f3ff-6742-4898-b8d7-317bf2004a58",
          "name": "blogger.comments.markAsSpam",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/posts/:postId/comments/:commentId/spam"
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
            "description": "Marks a comment as spam"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e51dda1-6b18-40d0-ad48-c95c294feec4"
            }
          ]
        }
      ]
    }
  ]
}