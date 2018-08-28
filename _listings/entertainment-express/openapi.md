swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 1
info:
  title: Entertainment Express
  description: your-gateway-to-building-incredible-movie-tv-and-game-content-discovery-experiences-
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