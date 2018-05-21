{
  "info": {
    "name": "Blogger API Get Blog Comments",
    "_postman_id": "40074bc5-6563-443a-a748-b7c82cdca615",
    "description": "Retrieves the comments for a blog, across all posts, possibly filtered.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "97d98759-6947-4f81-abf2-ea0920db8f01",
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
              "id": "216bf375-c2d1-4ad4-b3ff-3b7d0332b12b"
            }
          ]
        },
        {
          "id": "20f787f6-c924-4400-b47a-40b1861c8658",
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
              "id": "189ed975-2bbb-472e-bdfb-fdd5690e68c6"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog Comment",
      "item": [
        {
          "id": "3f26e94d-6a40-4122-9d32-d3dfa20a8721",
          "name": "blogger.comments.listByBlog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/comments"
              ],
              "query": [
                {
                  "key": "endDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "fetchBodies",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status",
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
            "description": "Retrieves the comments for a blog, across all posts, possibly filtered."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d80702b-5fcb-43d5-b43a-33731e8711aa"
            }
          ]
        }
      ]
    }
  ]
}