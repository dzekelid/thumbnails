---
swagger: "2.0"
x-collection-name: Firebase
x-complete: 0
info:
  title: Firebase Get Thumbnails
  description: |-
    Lists thumbnails of images attached to a step.

    May return any of the following canonical error codes: - PERMISSION_DENIED - if the user is not authorized to read from the project, or from any of the images - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the step does not exist, or if any of the images do not exist
  version: 1.0.0
host: '{project_id].firebaseio.co}'
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{projectId}/histories/{historyId}/executions/{executionId}/steps/{stepId}/thumbnails:
    get:
      summary: Get Thumbnails
      description: |-
        Lists thumbnails of images attached to a step.

        May return any of the following canonical error codes: - PERMISSION_DENIED - if the user is not authorized to read from the project, or from any of the images - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the step does not exist, or if any of the images do not exist
      operationId: toolresults.projects.histories.executions.steps.thumbnails.list
      x-api-path-slug: projectidhistorieshistoryidexecutionsexecutionidstepsstepidthumbnails-get
      parameters:
      - in: path
        name: executionId
        description: An Execution id
      - in: path
        name: historyId
        description: A History id
      - in: query
        name: pageSize
        description: The maximum number of thumbnails to fetch
      - in: query
        name: pageToken
        description: A continuation token to resume the query at the next item
      - in: path
        name: projectId
        description: A Project id
      - in: path
        name: stepId
        description: A Step id
      responses:
        200:
          description: OK
      tags:
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