---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /drive/root/thumbnails/{id}:
    get:
      summary: Get Thumbnail Set
      description: Get thumbnailSet Retrieve the properties and relationships of a
        thumbnailSet object.
      operationId: GetThumbnailSet
      x-api-path-slug: driverootthumbnailsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thumbnail
      - Set
  /drive/items/{id}/thumbnails/{id}:
    get:
      summary: Get Thumbnail Set
      description: Get thumbnailSet Retrieve the properties and relationships of a
        thumbnailSet object.
      operationId: GetThumbnailSet
      x-api-path-slug: driveitemsidthumbnailsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thumbnail
      - Set
  /drives/{id}/root/thumbnails/{id}:
    get:
      summary: Get Thumbnail Set
      description: Get thumbnailSet Retrieve the properties and relationships of a
        thumbnailSet object.
      operationId: GetThumbnailSet
      x-api-path-slug: drivesidrootthumbnailsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Thumbnail
      - Set
  /me/drive/root:/{item-path}:/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: medriverootitempaththumbnails-get
      parameters:
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /me/drive/items/{item-id}/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: medriveitemsitemidthumbnails-get
      parameters:
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /groups/{group-id}/drive/items/{item-id}/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidthumbnails-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
---