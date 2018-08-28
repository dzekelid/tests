---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Returns translated time from IVA or an error if invalid.
  description: Entertainment Express APIs use date time format ISO 8601.  Use this
    API to test your date time format to see if it translates to a valid time on our
    server.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Tests/TestDateTime/:
    get:
      summary: Returns translated time from IVA or an error if invalid.
      description: Entertainment Express APIs use date time format ISO 8601.  Use
        this API to test your date time format to see if it translates to a valid
        time on our server.
      operationId: GetTestDateTime
      x-api-path-slug: teststestdatetime-get
      parameters:
      - in: query
        name: DateTime
        description: DateTime to test format from API
      responses:
        200:
          description: OK
      tags:
      - Tests
      - TestDateTime
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