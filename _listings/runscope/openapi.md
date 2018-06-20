---
swagger: "2.0"
x-collection-name: Runscope
x-complete: 1
info:
  title: Runscope
  description: manage-runscope-programmatically-
  version: 1.0.0
host: api.runscope.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /buckets/{bucketKey}/tests:
    get:
      summary: Get Buckets Tests
      description: Returns a list of tests.
      operationId: buckets.bucketKey.tests.get
      x-api-path-slug: bucketsbucketkeytests-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
    post:
      summary: Add Buckets Tests
      description: Create a test.
      operationId: buckets.bucketKey.tests.post
      x-api-path-slug: bucketsbucketkeytests-post
      parameters:
      - in: body
        name: NewTest
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
  /buckets/{bucketKey}/tests/{testId}:
    delete:
      summary: Delete Buckets Tests
      description: Delete a test, including all steps, schedules, test-specific environments
        and results.
      operationId: buckets.bucketKey.tests.testId.delete
      x-api-path-slug: bucketsbucketkeyteststestid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
    get:
      summary: Get Buckets Tests
      description: Retrieve the details of a given test by ID.
      operationId: buckets.bucketKey.tests.testId.get
      x-api-path-slug: bucketsbucketkeyteststestid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
    put:
      summary: Put Buckets Tests
      description: Modify a test's name, description, default environment and its
        steps. To modify other individual properties of a test, make requests to the
        steps, environments, and schedules subresources of the test.
      operationId: buckets.bucketKey.tests.testId.put
      x-api-path-slug: bucketsbucketkeyteststestid-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
  /buckets/{bucketKey}/tests/{testId}/environments:
    get:
      summary: Get Buckets Tests Environments
      description: Return details of the test's environments (only those that belong
        to the specified test)
      operationId: buckets.bucketKey.tests.testId.environments.get
      x-api-path-slug: bucketsbucketkeyteststestidenvironments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Environments
    post:
      summary: Add Buckets Tests Environments
      description: Create new test environment.
      operationId: buckets.bucketKey.tests.testId.environments.post
      x-api-path-slug: bucketsbucketkeyteststestidenvironments-post
      parameters:
      - in: body
        name: NewEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Environments
  /buckets/{bucketKey}/tests/{testId}/environments/{environmentId}:
    put:
      summary: Put Buckets Tests Environments
      description: Update the details of a test environment.
      operationId: buckets.bucketKey.tests.testId.environments.environmentId.put
      x-api-path-slug: bucketsbucketkeyteststestidenvironmentsenvironmentid-put
      parameters:
      - in: body
        name: ModifiedEnvironment
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Environments
  /buckets/{bucketKey}/tests/{testId}/metrics:
    get:
      summary: Get Buckets Tests Metrics
      description: Return details of the test metrics for the specified timeframe.
      operationId: buckets.bucketKey.tests.testId.metrics.get
      x-api-path-slug: bucketsbucketkeyteststestidmetrics-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Metrics
  /buckets/{bucketKey}/tests/{testId}/steps:
    get:
      summary: Get Buckets Tests Steps
      description: List test steps for a test.
      operationId: buckets.bucketKey.tests.testId.steps.get
      x-api-path-slug: bucketsbucketkeyteststestidsteps-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
    post:
      summary: Add Buckets Tests Steps
      description: Add new test step.
      operationId: buckets.bucketKey.tests.testId.steps.post
      x-api-path-slug: bucketsbucketkeyteststestidsteps-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: TestStep
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
  /buckets/{bucketKey}/tests/{testId}/steps/{stepId}:
    delete:
      summary: Delete Buckets Tests Steps
      description: Delete a step from a test.
      operationId: buckets.bucketKey.tests.testId.steps.stepId.delete
      x-api-path-slug: bucketsbucketkeyteststestidstepsstepid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
    put:
      summary: Put Buckets Tests Steps
      description: Update the details of a single test step.
      operationId: buckets.bucketKey.tests.testId.steps.stepId.put
      x-api-path-slug: bucketsbucketkeyteststestidstepsstepid-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: TestStep
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Buckets
      - Tests
      - Steps
---