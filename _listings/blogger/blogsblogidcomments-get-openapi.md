---
swagger: "2.0"
x-collection-name: Blogger
x-complete: 0
info:
  title: Blogger API Get Blog Comments
  description: Retrieves the comments for a blog, across all posts, possibly filtered.
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
  /blogs/{blogId}:
    get:
      summary: Get Blog
      description: Gets one blog by ID.
      operationId: blogger.blogs.get
      x-api-path-slug: blogsblogid-get
      parameters:
      - in: path
        name: blogId
        description: The ID of the blog to get
      - in: query
        name: maxPosts
        description: Maximum number of posts to pull back with the blog
      - in: query
        name: view
        description: Access level with which to view the blog
      responses:
        200:
          description: OK
      tags:
      - Blog
  /blogs/{blogId}/comments:
    get:
      summary: Get Blog Comments
      description: Retrieves the comments for a blog, across all posts, possibly filtered.
      operationId: blogger.comments.listByBlog
      x-api-path-slug: blogsblogidcomments-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch comments from
      - in: query
        name: endDate
        description: Latest date of comment to fetch, a date-time with RFC 3339 formatting
      - in: query
        name: fetchBodies
        description: Whether the body content of the comments is included
      - in: query
        name: maxResults
        description: Maximum number of comments to include in the result
      - in: query
        name: pageToken
        description: Continuation token if request is paged
      - in: query
        name: startDate
        description: Earliest date of comment to fetch, a date-time with RFC 3339
          formatting
      - in: query
        name: status
      responses:
        200:
          description: OK
      tags:
      - Blog Comment
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