---
swagger: "2.0"
x-collection-name: CircleCI
x-complete: 1
info:
  title: CircleCI
  description: the-circleci-api-is-a-restful-fullyfeatured-api-that-allows-you-to-do-almost-anything-in-circleci--you-can-access-all-information-and-trigger-all-actions--the-only-thing-we-dont-provide-access-to-is-billing-functions-which-must-be-done-from-the-circleci-web-ui-
  version: 1.0.0
host: circleci.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /project/{username}/{project}/{build_num}/tests:
    get:
      summary: Get Project Username Project Build Num Tests
      description: |-
        Provides test metadata for a build
        Note: [Learn how to set up your builds to collect test metadata](https://circleci.com/docs/test-metadata/)
      operationId: getProjectUsernameProjectBuildNumTests
      x-api-path-slug: projectusernameprojectbuild-numtests-get
      responses:
        200:
          description: OK
      tags:
      - Project
      - Username
      - Project
      - Build
      - Num
      - Tests
    parameters:
      summary: Parameters Project Username Project Build Num Tests
      description: Parameters project username project build num tests.
      operationId: parametersProjectUsernameProjectBuildNumTests
      x-api-path-slug: projectusernameprojectbuild-numtests-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Project
      - Username
      - Project
      - Build
      - Num
      - Tests
---