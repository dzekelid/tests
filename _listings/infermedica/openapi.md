swagger: "2.0"
x-collection-name: Infermedica
x-complete: 1
info:
  title: Infermedica
  description: empower-your-healthcare-services-with-intelligent-diagnostic-insights-of-infermedica-api-
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