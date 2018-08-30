{
  "info": {
    "name": "Blogger API Get Blog Post Comment",
    "_postman_id": "d9b927ce-821e-48d2-b6e2-9cad8573bc65",
    "description": "Gets one comment by ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "comments",
      "item": [
        {
          "id": "283d489c-1b71-4447-98bc-01d5c7b55248",
          "name": "blogger.comments.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/posts/:postId/comments/:commentId"
              ],
              "query": [
                {
                  "key": "view",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets one comment by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44a21c08-59c6-4d62-a378-ffcf130369ea"
            }
          ]
        }
      ]
    }
  ]
}