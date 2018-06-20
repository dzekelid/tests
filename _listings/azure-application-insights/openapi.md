---
swagger: "2.0"
x-collection-name: Azure Application Insights
x-complete: 1
info:
  title: Application Insights API
  description: application-insights-in-preview-is-an-allinone-telemetry-solution-that-can-help-you-detect-issues-triage-impact-and-solve-problems-in-your-web-apps-and-services--it-provides-deep-diagnostics-and-realtime-insights-while-being-a-seamless-part-of-your-alm-processes-through-visual-studio-visual-studio-team-services-and-azure-diagnostics-integrations--it-supports-asp-net-j2ee-and-most-of-the-popular-web-technologies-for-web-apps-on-azure-or-on-your-own-servers-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests:
    get:
      summary: Web Tests By Resource Group
      description: Get all Application Insights web tests defined within a specified
        resource group.
      operationId: WebTests_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtests-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Web Tests
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests/{webTestName}:
    get:
      summary: Get Web Tests
      description: Get a specific Application Insights web test definition.
      operationId: WebTests_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Web Tests
    put:
      summary: Create or Update Web Tests
      description: Creates or updates an Application Insights web test definition.
      operationId: WebTests_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: WebTestDefinition
        description: Properties that need to be specified to create or update an Application
          Insights web test definition
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Web Tests
    patch:
      summary: Update Web Tests Tags
      description: Creates or updates an Application Insights web test definition.
      operationId: WebTests_UpdateTags
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-patch
      parameters:
      - in: query
        name: No Name
      - in: body
        name: WebTestTags
        description: Updated tag information to set into the web test instance
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Web Tests
    delete:
      summary: Delete Web Tests
      description: Deletes an Application Insights web test.
      operationId: WebTests_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Web Tests
  /subscriptions/{subscriptionId}/providers/microsoft.insights/webtests:
    get:
      summary: List Web Tests
      description: Get all Application Insights web test alerts definitioned within
        a subscription.
      operationId: WebTests_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-insightswebtests-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Web Tests
---