---
swagger: "2.0"
x-collection-name: Entertainment Express
x-complete: 0
info:
  title: Entertainment Express Get Viewers by Platform Hardware.
  description: No required parameters, DateValue defaults to Today.
  version: "2.0"
host: ee.iva-api.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Analytics/City/:
    get:
      summary: Get Viewers by City.
      description: No required parameters, DateValue defaults to Today..
      operationId: GetAnalyticsViewersByCity
      x-api-path-slug: analyticscity-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - City
  /Analytics/Country/:
    get:
      summary: Get Viewers by Country.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByCountry
      x-api-path-slug: analyticscountry-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - Country
  /Analytics/EngagementActions/:
    get:
      summary: GetAnalyticEngagementActions
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticEngagementActions
      x-api-path-slug: analyticsengagementactions-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - EngagementActions
  /Analytics/EngagementTimes/:
    get:
      summary: Get View count by Frequency.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsEngagementTimes
      x-api-path-slug: analyticsengagementtimes-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - EngagementTimes
  /Analytics/GBUsage/:
    get:
      summary: Get GBUsage by Customer ID.
      description: Requires a valid Customer ID.
      operationId: GetAnalyticsGBUsage
      x-api-path-slug: analyticsgbusage-get
      parameters:
      - in: query
        name: Month
        description: Report month
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Year
        description: Report year
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - GBUsage
  /Analytics/MostActive/:
    get:
      summary: Get Most Active Visitors by IP.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsMostActive
      x-api-path-slug: analyticsmostactive-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - MostActive
  /Analytics/PlatformHardware/:
    get:
      summary: Get Viewers by Platform Hardware.
      description: No required parameters, DateValue defaults to Today.
      operationId: GetAnalyticsViewersByPlatformHardware
      x-api-path-slug: analyticsplatformhardware-get
      parameters:
      - in: query
        name: DateValue
        description: Days spanned by report
      - in: query
        name: End
        description: Report end date
      - in: query
        name: Limit
        description: Number of records returned from top of response
      - in: query
        name: ReportTag
        description: Report Tag filter
      - in: query
        name: Start
        description: Report start date
      responses:
        200:
          description: OK
      tags:
      - Analytics
      - PlatformHardware
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