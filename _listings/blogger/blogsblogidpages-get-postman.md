{
  "info": {
    "name": "Blogger API Get Blog Pages",
    "_postman_id": "e37f880e-d284-4673-a684-00039d81e6a0",
    "description": "Retrieves the pages for a blog, optionally including non-LIVE statuses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Blog",
      "item": [
        {
          "id": "0148c077-97c9-4a4a-baf8-073fdfde4eba",
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
              "id": "85f0e503-2366-43d3-b0a0-31dda0cd67b5"
            }
          ]
        },
        {
          "id": "1a0f9221-8e80-4de1-aefb-be41bfce1dec",
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
              "id": "c2851981-d935-49c3-8b94-05a38b7c3cfb"
            }
          ]
        }
      ]
    },
    {
      "name": "Blog Comment",
      "item": [
        {
          "id": "b54df9cb-f7f2-4a4b-bd69-4f62480921f4",
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
              "id": "b5a2075a-9d7f-433a-841e-34bdbc1e8d81"
            }
          ]
        }
      ]
    },
    {
      "name": "Page",
      "item": [
        {
          "id": "88daa788-ba53-4925-911c-9103e17686c7",
          "name": "blogger.pages.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "blogger",
                "v3",
                "blogs/:blogId/pages"
              ],
              "query": [
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
                  "key": "status",
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
            "description": "Retrieves the pages for a blog, optionally including non-LIVE statuses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cf58e19-19d6-48a1-a87f-f41e29bddaa4"
            }
          ]
        }
      ]
    }
  ]
}