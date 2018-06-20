---
swagger: "2.0"
x-collection-name: AWS Pinpoint
x-complete: 1
info:
  title: AWS Pinpoint API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps/application-id/segments:
    get:
      summary: Segments List
      description: Use the GET method to request information about your segments.
      operationId: segmentsList
      x-api-path-slug: appsapplicationidsegments-get
      responses:
        200:
          description: OK
      tags:
      - Segments
    post:
      summary: Segments List
      description: Use the POST method to create or update a segment.
      operationId: addSegmentsList
      x-api-path-slug: appsapplicationidsegments-post
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/segments/segment-id:
    get:
      summary: Segment Instance
      description: Use the GET method to request information about a segment.
      operationId: getSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-get
      responses:
        200:
          description: OK
      tags:
      - Segments
    put:
      summary: Segment Instance
      description: Use the PUT method to update a segment.
      operationId: updateSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-put
      responses:
        200:
          description: OK
      tags:
      - Segments
    delete:
      summary: Segment Instance
      description: Use the DELETE method to delete a segment.
      operationId: deleteSegmentInstance
      x-api-path-slug: appsapplicationidsegmentssegmentid-delete
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/segment/versions:
    get:
      summary: Segment Versions List
      description: Use the GET method to request information about your segment versions.
      operationId: getSegmentVersionsList
      x-api-path-slug: appsapplicationidsegmentversions-get
      responses:
        200:
          description: OK
      tags:
      - Segments
  /apps/application-id/segments/segment-id/versions/version:
    get:
      summary: Segment Version Instance
      description: Use the GET method to request information about a segment version.
      operationId: getSegmentVersionInstance
      x-api-path-slug: appsapplicationidsegmentssegmentidversionsversion-get
      responses:
        200:
          description: OK
      tags:
      - Segments
---