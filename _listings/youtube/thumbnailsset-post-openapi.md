---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Add Thumbnails Set
  description: Uploads a custom video thumbnail to YouTube and sets it for a video.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /thumbnails/set:
    post:
      summary: Add Thumbnails Set
      description: Uploads a custom video thumbnail to YouTube and sets it for a video.
      operationId: postThumbnailsSet
      x-api-path-slug: thumbnailsset-post
      parameters:
      - in: query
        name: onBehalfOfContentOwner
        description: 'Note: This parameter is intended exclusively for YouTube content
          partners'
      - in: query
        name: videoId
        description: The videoId parameter specifies a YouTube video ID for which
          the custom video thumbnail is being provided
      responses:
        200:
          description: OK
      tags:
      - Thumbnails
      - Set
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