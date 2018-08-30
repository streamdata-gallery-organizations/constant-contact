---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Update Campaign
  description: Update Campaign
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/activities:
    get:
      summary: List Activities
      description: List Activities
      operationId: list-activities
      x-api-path-slug: usernameactivities-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Activities
    post:
      summary: Add Activity
      description: Add Activity
      operationId: add-activity
      x-api-path-slug: usernameactivities-post
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Activity
  /{username}/activities/{activity-id}:
    get:
      summary: Get Activity
      description: Get Activity
      operationId: get-activity
      x-api-path-slug: usernameactivitiesactivityid-get
      parameters:
      - in: path
        name: activity-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Activity
  /{username}/campaigns:
    get:
      summary: List Campaigns
      description: List Campaigns
      operationId: list-campaigns
      x-api-path-slug: usernamecampaigns-get
      parameters:
      - in: query
        name: refresh
        description: To initiate re-calculation of campaign results, you must use
          refresh= true
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Campaigns
    post:
      summary: Add Campaign
      description: Add Campaign
      operationId: add-campaign
      x-api-path-slug: usernamecampaigns-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
  /{username}/campaigns/{campaign-id}:
    delete:
      summary: Delete Campaign
      description: Delete Campaign
      operationId: delete-campaign
      x-api-path-slug: usernamecampaignscampaignid-delete
      parameters:
      - in: path
        name: campaign-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
    get:
      summary: Get Campaign
      description: Get Campaign
      operationId: get-campaign
      x-api-path-slug: usernamecampaignscampaignid-get
      parameters:
      - in: path
        name: campaign-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
    put:
      summary: Update Campaign
      description: Update Campaign
      operationId: update-campaign
      x-api-path-slug: usernamecampaignscampaignid-put
      parameters:
      - in: path
        name: campaign-id
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
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