---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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
---