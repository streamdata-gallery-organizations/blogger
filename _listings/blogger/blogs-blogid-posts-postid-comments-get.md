---
swagger: "2.0"
info:
  title: Blogger
  description: API for access to the data within Blogger.
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
  /blogs/{blogId}/posts/{postId}/comments:
    get:
      summary: Get Blog Post Comments
      description: Retrieves the comments for a post, possibly filtered
      operationId: blogger.comments.list
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
      - in: path
        name: postId
        description: ID of the post to fetch posts from
      - in: query
        name: startDate
        description: Earliest date of comment to fetch, a date-time with RFC 3339
          formatting
      - in: query
        name: status
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
      - comments
definitions:
  Blog:
    properties:
      customMetaData:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      locale:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      pages:
        description: This is a default description.
        type: parameters
      posts:
        description: This is a default description.
        type: parameters
      published:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  BlogList:
    properties:
      blogUserInfos:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  BlogPerUserInfo:
    properties:
      blogId:
        description: This is a default description.
        type: parameters
      hasAdminAccess:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      photosAlbumKey:
        description: This is a default description.
        type: parameters
      role:
        description: This is a default description.
        type: parameters
      userId:
        description: This is a default description.
        type: parameters
  BlogUserInfo:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  Comment:
    properties:
      author:
        description: This is a default description.
        type: parameters
      blog:
        description: This is a default description.
        type: parameters
      content:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      inReplyTo:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      post:
        description: This is a default description.
        type: parameters
      published:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  CommentList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      prevPageToken:
        description: This is a default description.
        type: parameters
  Page:
    properties:
      author:
        description: This is a default description.
        type: parameters
      blog:
        description: This is a default description.
        type: parameters
      content:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      published:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  PageList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  Pageviews:
    properties:
      blogId:
        description: This is a default description.
        type: parameters
      counts:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Post:
    properties:
      author:
        description: This is a default description.
        type: parameters
      blog:
        description: This is a default description.
        type: parameters
      content:
        description: This is a default description.
        type: parameters
      customMetaData:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      images:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      labels:
        description: This is a default description.
        type: parameters
      location:
        description: This is a default description.
        type: parameters
  PostList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  PostPerUserInfo:
    properties:
      blogId:
        description: This is a default description.
        type: parameters
      hasEditAccess:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      postId:
        description: This is a default description.
        type: parameters
      userId:
        description: This is a default description.
        type: parameters
  PostUserInfo:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  PostUserInfosList:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  User:
    properties:
      about:
        description: This is a default description.
        type: parameters
      blogs:
        description: This is a default description.
        type: parameters
      created:
        description: This is a default description.
        type: parameters
      displayName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      locale:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      url:
        description: This is a default description.
        type: parameters
x-collection-name: Blogger
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