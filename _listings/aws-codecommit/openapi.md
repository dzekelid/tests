swagger: "2.0"
x-collection-name: AWS CodeCommit
x-complete: 1
info:
  title: AWS CodeCommit API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TestRepositoryTriggers:
    get:
      summary: Test Repository Triggers
      description: Tests the functionality of repository triggers by sending information
        to the trigger target.
      operationId: testRepositoryTriggers
      x-api-path-slug: actiontestrepositorytriggers-get
      parameters:
      - in: query
        name: repositoryName
        description: The name of the repository in which to test the triggers
        type: string
      - in: query
        name: triggers
        description: The list of triggers to test
        type: string
      responses:
        200:
          description: OK
      tags:
      - Repository Triggers