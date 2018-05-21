---
swagger: "2.0"
x-collection-name: Blogger
x-complete: 0
info:
  title: Blogger API Get Blog by URL
  description: Retrieve a Blog by URL.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /blogger/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blogs/byurl:
    get:
      summary: Get Blog by URL
      description: Retrieve a Blog by URL.
      operationId: blogger.blogs.getByUrl
      x-api-path-slug: blogsbyurl-get
      parameters:
      - in: query
        name: url
        description: The URL of the blog to retrieve
      - in: query
        name: view
        description: Access level with which to view the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---