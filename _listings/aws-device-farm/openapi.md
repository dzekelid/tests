swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetTest:
    get:
      summary: Get Test
      description: Gets information about a test.
      operationId: getTest
      x-api-path-slug: actiongettest-get
      parameters:
      - in: query
        name: arn
        description: The tests ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tests
  /?Action=ListTests:
    get:
      summary: List Tests
      description: Gets information about tests.
      operationId: listTests
      x-api-path-slug: actionlisttests-get
      parameters:
      - in: query
        name: arn
        description: The tests ARNs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tests