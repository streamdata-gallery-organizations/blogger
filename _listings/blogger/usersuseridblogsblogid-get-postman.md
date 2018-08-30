{
  "info": {
    "name": "Blogger API Get User Blog",
    "_postman_id": "f2aa7edd-98c1-48ce-a002-0ca11f351f6a",
    "description": "Gets one blog and user info pair by blogId and userId.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "user blogs",
      "item": [
        {
          "id": "1b64f9e6-5ddb-4515-9166-3d5cae7796ff",
          "name": "blogger.blogUserInfos.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "users/:userId/blogs/:blogId"
              ],
              "query": [
                {
                  "key": "maxPosts",
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
                  "id": "userId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets one blog and user info pair by blogId and userId"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c51c36be-2ced-428a-83ee-f7140ce19ebd"
            }
          ]
        }
      ]
    }
  ]
}