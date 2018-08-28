---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Content Gets a thumbnail for an image.
  description: |-
    Gets a thumbnail for an image.

    This method currently supports files with the following file extensions: .jpg, .jpeg, .png, .tiff, .tif, .gif, .bmp

    Photos that are larger than 20MB in size won't be converted to a thumbnail.
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-content.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /thumbnails/{root}/{path}:
    get:
      summary: Gets a thumbnail for an image.
      description: |-
        Gets a thumbnail for an image.

        This method currently supports files with the following file extensions: .jpg, .jpeg, .png, .tiff, .tif, .gif, .bmp

        Photos that are larger than 20MB in size won't be converted to a thumbnail.
      operationId: gets-a-thumbnail-for-an-imagethis-method-currently-supports-files-with-the-following-file-extensions
      x-api-path-slug: thumbnailsrootpath-get
      parameters:
      - in: query
        name: format
        description: For images that are photos, `jpeg` (default) should be preferred,
          while `png` is better for screenshots and digital art
      - in: path
        name: path
        description: The path to the image file you want to thumbnail
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      - in: query
        name: size
        description: Default size is `s`
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Thumbnails
      - Root
      - Path
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