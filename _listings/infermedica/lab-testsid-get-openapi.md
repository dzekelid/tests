---
swagger: "2.0"
x-collection-name: Infermedica
x-complete: 0
info:
  title: Infermedica Get Lab Tests
  description: Returns details of a single lab test specified by id parameter.
  version: v2
host: api.infermedica.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lab_tests:
    get:
      summary: Get Lab Tests
      description: Returns a list of all available lab tests.
      operationId: getLabTests
      x-api-path-slug: lab-tests-get
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Lab
      - Tests
  /lab_tests/{id}:
    get:
      summary: Get Lab Tests
      description: Returns details of a single lab test specified by id parameter.
      operationId: getLabTests
      x-api-path-slug: lab-testsid-get
      parameters:
      - in: path
        name: id
        description: lab test id
      responses:
        200:
          description: OK
      tags:
      - Healthcare
      - Lab
      - Tests
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