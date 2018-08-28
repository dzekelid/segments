swagger: "2.0"
x-collection-name: Google Analytics
x-complete: 1
info:
  title: Google Analytics
  description: views-and-manages-your-google-analytics-data-
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /analytics/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /management/segments:
    get:
      summary: Get Segments
      description: Lists segments to which the user has access.
      operationId: analytics.management.segments.list
      x-api-path-slug: managementsegments-get
      parameters:
      - in: query
        name: max-results
        description: The maximum number of segments to include in this response
      - in: query
        name: start-index
        description: An index of the first segment to retrieve
      responses:
        200:
          description: OK
      tags:
      - Segment