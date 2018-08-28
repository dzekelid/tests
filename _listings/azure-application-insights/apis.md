---
name: Azure Application Insights
x-slug: azure-application-insights
description: Get rich performance monitoring, powerful alerting, and easy-to-consume
  dashboards to help ensure your applications are available and performing as you
  expect. Quickly see if you have a problem, how many customers are affected, and
  perform a root cause analysis to find and fix the issue.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Tests
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Application Insights API Web Tests By Resource Group
  x-api-slug: azure-application-insights-api
  description: Get all Application Insights web tests defined within a specified resource
    group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
  humanURL: https://azure.microsoft.com/en-us/services/application-insights/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests
  tags: Web Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtests-get-openapi.md
- name: Azure Application Insights API Get Web Tests
  x-api-slug: azure-application-insights-api
  description: Get a specific Application Insights web test definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
  humanURL: https://azure.microsoft.com/en-us/services/application-insights/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests/{webTestName}
  tags: Web Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-get-openapi.md
- name: Azure Application Insights API Create or Update Web Tests
  x-api-slug: azure-application-insights-api
  description: Creates or updates an Application Insights web test definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
  humanURL: https://azure.microsoft.com/en-us/services/application-insights/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests/{webTestName}
  tags: Web Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-put-openapi.md
- name: Azure Application Insights API Update Web Tests Tags
  x-api-slug: azure-application-insights-api
  description: Creates or updates an Application Insights web test definition.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
  humanURL: https://azure.microsoft.com/en-us/services/application-insights/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests/{webTestName}
  tags: Web Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-patch-openapi.md
- name: Azure Application Insights API Delete Web Tests
  x-api-slug: azure-application-insights-api
  description: Deletes an Application Insights web test.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
  humanURL: https://azure.microsoft.com/en-us/services/application-insights/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests/{webTestName}
  tags: Web Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightswebtestswebtestname-delete-openapi.md
- name: Azure Application Insights API List Web Tests
  x-api-slug: azure-application-insights-api
  description: Get all Application Insights web test alerts definitioned within a
    subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
  humanURL: https://azure.microsoft.com/en-us/services/application-insights/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/microsoft.insights/webtests
  tags: Web Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/subscriptionssubscriptionidprovidersmicrosoft-insightswebtests-get-openapi.md
- name: Azure Application Insights API
  x-api-slug: azure-application-insights-api
  description: Application Insights (in preview) is an all-in-one telemetry solution
    that can help you detect issues, triage impact and solve problems in your web
    apps and services. It provides deep diagnostics and real-time insights while being
    a seamless part of your ALM processes through Visual Studio, Visual Studio Team
    Services, and Azure Diagnostics integrations. It supports ASP.NET, J2EE and most
    of the popular web technologies for web apps on Azure or on your own servers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/performance-management.png
  humanURL: https://azure.microsoft.com/en-us/services/application-insights/
  baseURL: ://management.azure.com//
  tags: Tests
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/tests/master/_listings/azure-application-insights/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/application-insights/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/application-insights/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/application-insights/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/application-insights/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---