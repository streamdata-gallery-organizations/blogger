{
  "info": {
    "name": "Blogger API Get Blog",
    "_postman_id": "b9bb33c1-08fc-441d-8e35-a4d019f99fad",
    "description": "Gets one blog by ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "a6b3ce27-081d-4a21-a54f-cec3d34caa5a",
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
              "id": "f9be1cb3-b4a2-46d4-befd-fa70557506bc"
            }
          ]
        },
        {
          "id": "8c61837e-0e8d-41fd-84a0-5ca7f35adc32",
          "name": "blogger.blogs.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId"
              ],
              "query": [
                {
                  "key": "maxPosts",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets one blog by ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "664b67b8-8dcf-4187-aaaa-cde951d4fd23"
            }
          ]
        }
      ]
    }
  ]
}