swagger: "2.0"
x-collection-name: BlazeMeter
x-complete: 1
info:
  title: Blazemeter API Explorer
  description: live-api-documentation
  version: 1.0.0
host: a.blazemeter.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/tests:
    get:
      summary: Get User Tests
      description: Get user tests.
      operationId: retrieveTests
      x-api-path-slug: usertests-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: skip
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Tests