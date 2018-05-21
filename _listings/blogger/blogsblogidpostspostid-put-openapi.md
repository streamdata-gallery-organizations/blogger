---
swagger: "2.0"
x-collection-name: Blogger
x-complete: 0
info:
  title: Blogger API Update Blog Post
  description: Update a post.
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
  /blogs/{blogId}/pages:
    get:
      summary: Get Blog Pages
      description: Retrieves the pages for a blog, optionally including non-LIVE statuses.
      operationId: blogger.pages.list
      x-api-path-slug: blogsblogidpages-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch Pages from
      - in: query
        name: fetchBodies
        description: Whether to retrieve the Page bodies
      - in: query
        name: maxResults
        description: Maximum number of Pages to fetch
      - in: query
        name: pageToken
        description: Continuation token if the request is paged
      - in: query
        name: status
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
      - Page
    post:
      summary: Add Blog Page
      description: Add a page.
      operationId: blogger.pages.insert
      x-api-path-slug: blogsblogidpages-post
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to add the page to
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: isDraft
        description: 'Whether to create the page as a draft (default: false)'
      responses:
        200:
          description: OK
      tags:
      - Page
  /blogs/{blogId}/pages/{pageId}:
    delete:
      summary: Delete Blog Page
      description: Delete a page by ID.
      operationId: blogger.pages.delete
      x-api-path-slug: blogsblogidpagespageid-delete
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: path
        name: pageId
        description: The ID of the Page
      responses:
        200:
          description: OK
      tags:
      - Page
    get:
      summary: Get Blog Page
      description: Gets one blog page by ID.
      operationId: blogger.pages.get
      x-api-path-slug: blogsblogidpagespageid-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog containing the page
      - in: path
        name: pageId
        description: The ID of the page to get
      - in: query
        name: view
      responses:
        200:
          description: OK
      tags:
      - Page
    patch:
      summary: Update Blog Page
      description: Update a page. This method supports patch semantics.
      operationId: blogger.pages.patch
      x-api-path-slug: blogsblogidpagespageid-patch
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: pageId
        description: The ID of the Page
      - in: query
        name: publish
        description: 'Whether a publish action should be performed when the page is
          updated (default: false)'
      - in: query
        name: revert
        description: 'Whether a revert action should be performed when the page is
          updated (default: false)'
      responses:
        200:
          description: OK
      tags:
      - Page
    put:
      summary: Update Blog Page
      description: Update a page.
      operationId: blogger.pages.update
      x-api-path-slug: blogsblogidpagespageid-put
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: pageId
        description: The ID of the Page
      - in: query
        name: publish
        description: 'Whether a publish action should be performed when the page is
          updated (default: false)'
      - in: query
        name: revert
        description: 'Whether a revert action should be performed when the page is
          updated (default: false)'
      responses:
        200:
          description: OK
      tags:
      - Page
  /blogs/{blogId}/pages/{pageId}/publish:
    post:
      summary: Publish Blog Page
      description: Publishes a draft page.
      operationId: blogger.pages.publish
      x-api-path-slug: blogsblogidpagespageidpublish-post
      parameters:
      - in: path
        name: blogId
        description: The ID of the blog
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Page
  /blogs/{blogId}/pages/{pageId}/revert:
    post:
      summary: Revert Blog Page
      description: Revert a published or scheduled page to draft state.
      operationId: blogger.pages.revert
      x-api-path-slug: blogsblogidpagespageidrevert-post
      parameters:
      - in: path
        name: blogId
        description: The ID of the blog
      - in: path
        name: pageId
        description: The ID of the page
      responses:
        200:
          description: OK
      tags:
      - Page
  /blogs/{blogId}/pageviews:
    get:
      summary: Get Blog Page Views
      description: Retrieve pageview stats for a Blog.
      operationId: blogger.pageViews.get
      x-api-path-slug: blogsblogidpageviews-get
      parameters:
      - in: path
        name: blogId
        description: The ID of the blog to get
      - in: query
        name: range
      responses:
        200:
          description: OK
      tags:
      - Page Views
  /blogs/{blogId}/posts:
    get:
      summary: Get Blog Posts
      description: Retrieves a list of posts, possibly filtered.
      operationId: blogger.posts.list
      x-api-path-slug: blogsblogidposts-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch posts from
      - in: query
        name: endDate
        description: Latest post date to fetch, a date-time with RFC 3339 formatting
      - in: query
        name: fetchBodies
        description: 'Whether the body content of posts is included (default: true)'
      - in: query
        name: fetchImages
        description: Whether image URL metadata for each post is included
      - in: query
        name: labels
        description: Comma-separated list of labels to search for
      - in: query
        name: maxResults
        description: Maximum number of posts to fetch
      - in: query
        name: orderBy
        description: Sort search results
      - in: query
        name: pageToken
        description: Continuation token if the request is paged
      - in: query
        name: startDate
        description: Earliest post date to fetch, a date-time with RFC 3339 formatting
      - in: query
        name: status
        description: Statuses to include in the results
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
      - Blog Post
    post:
      summary: Add Blog Post
      description: Add a post.
      operationId: blogger.posts.insert
      x-api-path-slug: blogsblogidposts-post
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to add the post to
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fetchBody
        description: 'Whether the body content of the post is included with the result
          (default: true)'
      - in: query
        name: fetchImages
        description: 'Whether image URL metadata for each post is included in the
          returned result (default: false)'
      - in: query
        name: isDraft
        description: 'Whether to create the post as a draft (default: false)'
      responses:
        200:
          description: OK
      tags:
      - Blog Post
  /blogs/{blogId}/posts/bypath:
    get:
      summary: Get Blog Post by Path
      description: Retrieve a Post by Path.
      operationId: blogger.posts.getByPath
      x-api-path-slug: blogsblogidpostsbypath-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch the post from
      - in: query
        name: maxComments
        description: Maximum number of comments to pull back on a post
      - in: query
        name: path
        description: Path of the Post to retrieve
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
      - Blog Post
  /blogs/{blogId}/posts/search:
    get:
      summary: Search Blog Post
      description: Search for a post.
      operationId: blogger.posts.search
      x-api-path-slug: blogsblogidpostssearch-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch the post from
      - in: query
        name: fetchBodies
        description: 'Whether the body content of posts is included (default: true)'
      - in: query
        name: orderBy
        description: Sort search results
      - in: query
        name: q
        description: Query terms to search this blog for matching posts
      responses:
        200:
          description: OK
      tags:
      - Blog Search
  /blogs/{blogId}/posts/{postId}:
    delete:
      summary: Delete Blog Post
      description: Delete a post by ID.
      operationId: blogger.posts.delete
      x-api-path-slug: blogsblogidpostspostid-delete
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: path
        name: postId
        description: The ID of the Post
      responses:
        200:
          description: OK
      tags:
      - Blog Post
    get:
      summary: Get Blog Post
      description: Get a post by ID.
      operationId: blogger.posts.get
      x-api-path-slug: blogsblogidpostspostid-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch the post from
      - in: query
        name: fetchBody
        description: 'Whether the body content of the post is included (default: true)'
      - in: query
        name: fetchImages
        description: 'Whether image URL metadata for each post is included (default:
          false)'
      - in: query
        name: maxComments
        description: Maximum number of comments to pull back on a post
      - in: path
        name: postId
        description: The ID of the post
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
      - Blog Post
    patch:
      summary: Update Blog Post
      description: Update a post. This method supports patch semantics.
      operationId: blogger.posts.patch
      x-api-path-slug: blogsblogidpostspostid-patch
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fetchBody
        description: 'Whether the body content of the post is included with the result
          (default: true)'
      - in: query
        name: fetchImages
        description: 'Whether image URL metadata for each post is included in the
          returned result (default: false)'
      - in: query
        name: maxComments
        description: Maximum number of comments to retrieve with the returned post
      - in: path
        name: postId
        description: The ID of the Post
      - in: query
        name: publish
        description: 'Whether a publish action should be performed when the post is
          updated (default: false)'
      - in: query
        name: revert
        description: 'Whether a revert action should be performed when the post is
          updated (default: false)'
      responses:
        200:
          description: OK
      tags:
      - Blog Post
    put:
      summary: Update Blog Post
      description: Update a post.
      operationId: blogger.posts.update
      x-api-path-slug: blogsblogidpostspostid-put
      parameters:
      - in: path
        name: blogId
        description: The ID of the Blog
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fetchBody
        description: 'Whether the body content of the post is included with the result
          (default: true)'
      - in: query
        name: fetchImages
        description: 'Whether image URL metadata for each post is included in the
          returned result (default: false)'
      - in: query
        name: maxComments
        description: Maximum number of comments to retrieve with the returned post
      - in: path
        name: postId
        description: The ID of the Post
      - in: query
        name: publish
        description: 'Whether a publish action should be performed when the post is
          updated (default: false)'
      - in: query
        name: revert
        description: 'Whether a revert action should be performed when the post is
          updated (default: false)'
      responses:
        200:
          description: OK
      tags:
      - Blog Post
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