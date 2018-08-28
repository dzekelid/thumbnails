---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Admin Event Eventid Thumbnail Url
  version: 1.0.0
  description: Post admin event eventid thumbnail url.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/event/{eventId}/thumbnail/url:
    post:
      summary: Post Admin Event Eventid Thumbnail Url
      description: Post admin event eventid thumbnail url.
      operationId: postApiV1AdminEventEventThumbnailUrl
      x-api-path-slug: apiv1admineventeventidthumbnailurl-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: body
        name: url
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Eventid
      - Thumbnail
      - Url
  /api/v1/admin/place/{placeId}/thumbnail:
    post:
      summary: Post Admin Place Placeid Thumbnail
      description: Post admin place placeid thumbnail.
      operationId: postApiV1AdminPlacePlaceThumbnail
      x-api-path-slug: apiv1adminplaceplaceidthumbnail-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Placeid
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