---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Datastore API Get Thumbnails
  description: /thumbnails
  version: "1"
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /thumbnails:
    get:
      summary: Get Thumbnails
      description: /thumbnails
      operationId: thumbnails
      x-api-path-slug: thumbnails-get
      parameters:
      - in: query
        name: format
        description: jpeg (default) or png
      - in: query
        name: size
        description: 'One of the following values (default: s):valuedimensions (px)xs32x32s64x64m128x128l640x480xl1024x768'
      responses:
        200:
          description: OK
      tags:
      - Thumbnails
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