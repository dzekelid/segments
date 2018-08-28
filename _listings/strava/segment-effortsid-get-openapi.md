---
swagger: "2.0"
x-collection-name: Strava
x-complete: 0
info:
  title: Strava Get Segment Effort
  description: Returns a segment effort from an activity that is owned by the authenticated
    athlete.
  version: 1.0.0
host: www.strava.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /segments/starred:
    get:
      summary: List Starred Segments
      description: List of the authenticated athlete's starred segments.
      operationId: getLoggedInAthleteStarredSegments
      x-api-path-slug: segmentsstarred-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Starred
      - Segments
  /segments/explore:
    get:
      summary: Explore segments
      description: Returns the top 10 segments matching a specified query.
      operationId: exploreSegments
      x-api-path-slug: segmentsexplore-get
      parameters:
      - in: query
        name: activity_type
        description: Desired activity type
      - in: query
        name: bounds
        description: 'The latitude and longitude for two points describing a rectangular
          boundary for the search: [southwest corner latitutde, southwest corner longitude,
          northeast corner latitude, northeast corner longitude]'
      - in: query
        name: max_cat
        description: The maximum climbing category
      - in: query
        name: min_cat
        description: The minimum climbing category
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Explore
      - Segments
  /segments/{id}:
    get:
      summary: Get Segment
      description: Returns the specified segment.
      operationId: getSegmentById
      x-api-path-slug: segmentsid-get
      parameters:
      - in: path
        name: id
        description: The identifier of the segment
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Segment
  /segments/{id}/starred:
    put:
      summary: Star Segment
      description: Stars/Unstars the given segment for the authenticated athlete.
      operationId: starSegment
      x-api-path-slug: segmentsidstarred-put
      parameters:
      - in: path
        name: id
        description: The identifier of the segment to star
      - in: formData
        name: starred
        description: If true, star the segment; if false, unstar the segment
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Star
      - Segment
  /segments/{id}/leaderboard:
    get:
      summary: Get Segment Leaderboard
      description: Returns the specified segment leaderboard.
      operationId: getLeaderboardBySegmentId
      x-api-path-slug: segmentsidleaderboard-get
      parameters:
      - in: query
        name: age_group
        description: Premium Feature
      - in: query
        name: club_id
        description: Filter by club
      - in: query
        name: context_entries
      - in: query
        name: date_range
        description: Filter by date range
      - in: query
        name: following
        description: Filter by friends of the authenticated athlete
      - in: query
        name: gender
        description: Filter by gender
      - in: path
        name: id
        description: The identifier of the segment leaderboard
      - in: query
        name: No Name
      - in: query
        name: weight_class
        description: Premium Feature
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Segment
      - Leaderboard
  /segments/{id}/all_efforts:
    get:
      summary: List Segment Efforts
      description: Returns a set of the authenticated athlete's segment efforts for
        a given segment.
      operationId: getEffortsBySegmentId
      x-api-path-slug: segmentsidall-efforts-get
      parameters:
      - in: path
        name: id
        description: The identifier of the segment
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - List
      - Segment
      - Efforts
  /segment_efforts/{id}:
    get:
      summary: Get Segment Effort
      description: Returns a segment effort from an activity that is owned by the
        authenticated athlete.
      operationId: getSegmentEffortById
      x-api-path-slug: segment-effortsid-get
      parameters:
      - in: path
        name: id
        description: The identifier of the segment effort
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Segment
      - Effort
  /segment_efforts/{id}/streams:
    get:
      summary: Get segment effort streams
      description: Returns a set of streams for a segment effort completed by the
        authenticated athlete.
      operationId: getSegmentEffortStreams
      x-api-path-slug: segment-effortsidstreams-get
      parameters:
      - in: path
        name: id
        description: The identifier of the segment effort
      - in: query
        name: keys
        description: The types of streams to return
      - in: query
        name: key_by_type
        description: Must be true
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Segment
      - Effort
      - Streams
  /segments/{id}/streams:
    get:
      summary: Get Segment Streams
      description: Returns the given segment's streams.
      operationId: getSegmentStreams
      x-api-path-slug: segmentsidstreams-get
      parameters:
      - in: path
        name: id
        description: The identifier of the segment
      - in: query
        name: keys
        description: The types of streams to return
      - in: query
        name: key_by_type
        description: Must be true
      responses:
        200:
          description: Successful response
      tags:
      - Sports
      - Segment
      - Streams
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