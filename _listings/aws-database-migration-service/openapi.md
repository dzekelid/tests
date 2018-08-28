swagger: "2.0"
x-collection-name: AWS Database Migration Service
x-complete: 1
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TestConnection:
    get:
      summary: Test Connection
      description: Tests the connection between the replication instance and the endpoint.
      operationId: testConnection
      x-api-path-slug: actiontestconnection-get
      parameters:
      - in: query
        name: EndpointArn
        description: The Amazon Resource Name (ARN) string that uniquely identifies
          the endpoint
        type: string
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - Connections