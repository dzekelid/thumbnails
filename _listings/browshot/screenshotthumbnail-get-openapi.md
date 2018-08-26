---
swagger: "2.0"
x-collection-name: Browshot
x-complete: 0
info:
  title: Browshot Retrieve a thumbnail image
  description: |-
    Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image "Not found" is sent.

    You can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300.
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /screenshot/thumbnail:
    get:
      summary: Retrieve a thumbnail image
      description: |-
        Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image "Not found" is sent.

        You can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300.
      operationId: GetThumbnail
      x-api-path-slug: screenshotthumbnail-get
      parameters:
      - in: query
        name: bottom
        description: bottom edge of the area to be cropped
      - in: query
        name: format
        description: image as PNG or JPEG
      - in: query
        name: height
        description: height of the thumbnail
      - in: query
        name: id
        description: screenshot ID
      - in: query
        name: left
        description: left edge of the area to be cropped
      - in: query
        name: quality
        description: JPEG quality factor (for JPEG thumbnails only)
      - in: query
        name: ratio
        description: Use fit to keep the original page ration, and fill to get a thumbnail
          for the exact width and height
      - in: query
        name: right
        description: right edge of the area to be cropped
      - in: query
        name: scale
        description: scale of the thumbnail
      - in: query
        name: shot
        description: get the second or third screenshot if multiple screenshots were
          requested
      - in: query
        name: top
        description: top edge of the area to be cropped
      - in: query
        name: width
        description: width of the thumbnail
      - in: query
        name: zoom
        description: zoom 1 to 100 percent
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - Thumbnail
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