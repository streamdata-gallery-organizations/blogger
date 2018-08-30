{
  "info": {
    "name": "Blogger API Search Blog Post",
    "_postman_id": "a5e03d55-c95a-4f99-ad3d-629dea98b6a8",
    "description": "Search for a post.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "blog search",
      "item": [
        {
          "id": "44f977b5-6199-4414-8993-b6c260982557",
          "name": "blogger.posts.search",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/posts/search"
              ],
              "query": [
                {
                  "key": "fetchBodies",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "orderBy",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "q",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "blogId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for a post"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d62455fa-d351-419c-b061-d071afab5b2d"
            }
          ]
        }
      ]
    }
  ]
}