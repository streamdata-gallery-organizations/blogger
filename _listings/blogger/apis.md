---
name: Blogger
x-slug: blogger
description: Blogger is a blog-publishing service that allows multi-user blogs with
  time-stamped entries. It was developed by Pyra Labs, which was bought by Google
  in 2003. Generally, the blogs are hosted by Google at a subdomain of blogspot.com.
  Blogs can also be hosted in the registered custom domain of the blogger (like www.example.com).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
x-kinRank: "9"
x-alexaRank: ""
tags: Blogger
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/apis.md
specificationVersion: "0.14"
apis:
- name: Blogger API Get Blog by URL
  x-api-slug: blogger-api
  description: Retrieve a Blog by URL.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/byurl
  tags: Blog
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsbyurl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsbyurl-get-openapi.md
- name: Blogger API Get Blog
  x-api-slug: blogger-api
  description: Gets one blog by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}
  tags: Blog
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogid-get-openapi.md
- name: Blogger API Get Blog Comments
  x-api-slug: blogger-api
  description: Retrieves the comments for a blog, across all posts, possibly filtered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/comments
  tags: Blog Comment
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidcomments-get-openapi.md
- name: Blogger API Get Blog Pages
  x-api-slug: blogger-api
  description: Retrieves the pages for a blog, optionally including non-LIVE statuses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages
  tags: Page
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpages-get-openapi.md
- name: Blogger API Add Blog Page
  x-api-slug: blogger-api
  description: Add a page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages
  tags: Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpages-post-openapi.md
- name: Blogger API Delete Blog Page
  x-api-slug: blogger-api
  description: Delete a page by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages/{pageId}
  tags: Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpagespageid-delete-openapi.md
- name: Blogger API Get Blog Page
  x-api-slug: blogger-api
  description: Gets one blog page by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages/{pageId}
  tags: Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpagespageid-get-openapi.md
- name: Blogger API Update Blog Page
  x-api-slug: blogger-api
  description: Update a page. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages/{pageId}
  tags: Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpagespageid-patch-openapi.md
- name: Blogger API Update Blog Page
  x-api-slug: blogger-api
  description: Update a page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages/{pageId}
  tags: Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpagespageid-put-openapi.md
- name: Blogger API Publish Blog Page
  x-api-slug: blogger-api
  description: Publishes a draft page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages/{pageId}/publish
  tags: Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpagespageidpublish-post-openapi.md
- name: Blogger API Revert Blog Page
  x-api-slug: blogger-api
  description: Revert a published or scheduled page to draft state.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pages/{pageId}/revert
  tags: Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpagespageidrevert-post-openapi.md
- name: Blogger API Get Blog Page Views
  x-api-slug: blogger-api
  description: Retrieve pageview stats for a Blog.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/pageviews
  tags: Page Views
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpageviews-get-openapi.md
- name: Blogger API Get Blog Posts
  x-api-slug: blogger-api
  description: Retrieves a list of posts, possibly filtered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidposts-get-openapi.md
- name: Blogger API Add Blog Post
  x-api-slug: blogger-api
  description: Add a post.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidposts-post-openapi.md
- name: Blogger API Get Blog Post by Path
  x-api-slug: blogger-api
  description: Retrieve a Post by Path.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/bypath
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostsbypath-get-openapi.md
- name: Blogger API Search Blog Post
  x-api-slug: blogger-api
  description: Search for a post.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/search
  tags: Blog Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostssearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostssearch-get-openapi.md
- name: Blogger API Delete Blog Post
  x-api-slug: blogger-api
  description: Delete a post by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostid-delete-openapi.md
- name: Blogger API Get Blog Post
  x-api-slug: blogger-api
  description: Get a post by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostid-get-openapi.md
- name: Blogger API Update Blog Post
  x-api-slug: blogger-api
  description: Update a post. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostid-patch-openapi.md
- name: Blogger API Update Blog Post
  x-api-slug: blogger-api
  description: Update a post.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostid-put-openapi.md
- name: Blogger API Get Blog Post Comments
  x-api-slug: blogger-api
  description: Retrieves the comments for a post, possibly filtered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcomments-get-openapi.md
- name: Blogger API Delete Blog Post Comments
  x-api-slug: blogger-api
  description: Delete a comment by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-delete-openapi.md
- name: Blogger API Get Blog Post Comment
  x-api-slug: blogger-api
  description: Gets one comment by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentid-get-openapi.md
- name: Blogger API Update Blog Post Comment
  x-api-slug: blogger-api
  description: Marks a comment as not spam.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}/approve
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentidapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentidapprove-post-openapi.md
- name: Blogger API Update Blog Post Comment
  x-api-slug: blogger-api
  description: Removes the content of a comment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}/removecontent
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentidremovecontent-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentidremovecontent-post-openapi.md
- name: Blogger API Update Blog Post Comment SPAM
  x-api-slug: blogger-api
  description: Marks a comment as spam.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/comments/{commentId}/spam
  tags: Comments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentidspam-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidcommentscommentidspam-post-openapi.md
- name: Blogger API Publish Blog Post
  x-api-slug: blogger-api
  description: Publishes a draft post, optionally at the specific time of the given
    publishDate parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/publish
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidpublish-post-openapi.md
- name: Blogger API Revert Blog Post
  x-api-slug: blogger-api
  description: Revert a published or scheduled post to draft state.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//blogs/{blogId}/posts/{postId}/revert
  tags: Blog Post
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/blogsblogidpostspostidrevert-post-openapi.md
- name: Blogger API Get User
  x-api-slug: blogger-api
  description: Gets one user by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//users/{userId}
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/usersuserid-get-openapi.md
- name: Blogger API Get User Blogs
  x-api-slug: blogger-api
  description: Retrieves a list of blogs, possibly filtered.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//users/{userId}/blogs
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/usersuseridblogs-get-openapi.md
- name: Blogger API Get User Blog
  x-api-slug: blogger-api
  description: Gets one blog and user info pair by blogId and userId.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//users/{userId}/blogs/{blogId}
  tags: User Blogs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/usersuseridblogsblogid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/usersuseridblogsblogid-get-openapi.md
- name: Blogger API Get User Blog Posts
  x-api-slug: blogger-api
  description: Retrieves a list of post and post user info pairs, possibly filtered.
    The post user info contains per-user information about the post, such as access
    rights, specific to the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//users/{userId}/blogs/{blogId}/posts
  tags: User Blog Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/usersuseridblogsblogidposts-get-openapi.md
- name: Blogger API Get User Blog Post
  x-api-slug: blogger-api
  description: Gets one post and user info pair, by post ID and user ID. The post
    user info contains per-user information about the post, such as access rights,
    specific to the user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3//users/{userId}/blogs/{blogId}/posts/{postId}
  tags: User Blog Posts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/usersuseridblogsblogidpostspostid-get-openapi.md
- name: Blogger API
  x-api-slug: blogger-api
  description: The Blogger API v3 allows client applications to view and update Blogger
    content. Your client application can use Blogger API v3 to create new blog posts,
    edit or delete existing posts, and query for posts that match particular criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blogger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/blogger/master/_listings/blogger/openapi.md
x-common:
- type: x-blog
  url: https://blogger.googleblog.com/
- type: x-website
  url: https://www.blogger.com
- type: x-blog-rss
  url: http://buzz.blogger.com/atom.xml
- type: x-developer
  url: https://developers.google.com/blogger/
- type: x-twitter
  url: https://twitter.com/Blogger
- type: x-getting-started
  url: https://developers.google.com/blogger/docs/3.0/getting_started
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---