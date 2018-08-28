swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{FILE_ID}/thumbnail.{EXTENSION}:
    get:
      summary: Get Thumbnail
      description: Retrieves a thumbnail, or smaller image representation, of this
        file. Sizes of 32x32,64x64, 128x128, and 256x256 can be returned in the .png
        format and sizes of 32x32, 94x94, 160x160, and 320x320 can be returned in
        the .jpg format. Thumbnails can be generated for the image and video file
        formats listed here.
      operationId: getFileThumbnail
      x-api-path-slug: filesfile-idthumbnail-extension-get
      parameters:
      - in: path
        name: EXTENSION
        description: The preview format, e
      - in: path
        name: FILE_ID
      - in: query
        name: max_height
        description: The maximum height of the thumbnail
      - in: query
        name: max_width
        description: The maximum width of the thumbnail
      - in: query
        name: min_height
        description: The minimum height of the thumbnail
      - in: query
        name: min_width
        description: The minimum width of the thumbnail
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Thumbnail.
      - Extension