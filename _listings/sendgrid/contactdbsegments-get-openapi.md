---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Contactdb Segments
  description: |-
    **This endpoint allows you to retrieve all of your segments.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

    For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contactdb/segments:
    get:
      summary: Get Contactdb Segments
      description: |-
        **This endpoint allows you to retrieve all of your segments.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.

        For more information about segments in Marketing Campaigns, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/lists.html#-Create-a-Segment).
      operationId: contactdb.segments.get
      x-api-path-slug: contactdbsegments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Segments
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