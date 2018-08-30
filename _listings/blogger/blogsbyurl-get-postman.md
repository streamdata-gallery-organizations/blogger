{
  "info": {
    "name": "Blogger API Get Blog by URL",
    "_postman_id": "6e3e9838-38af-43e2-a098-119a7ee48173",
    "description": "Retrieve a Blog by URL.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "492144b7-55b3-4fea-b1e2-c56ac6c5b4b6",
          "name": "blogger.blogs.getByUrl",
          "request": {
            "url": "http://www.googleapis.com/blogger/v3/blogs/byurl?url=%7B%7D&view=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a Blog by URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbed8c91-60d9-4f04-8956-c0de6e766c28"
            }
          ]
        }
      ]
    }
  ]
}