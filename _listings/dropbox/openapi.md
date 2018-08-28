swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
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