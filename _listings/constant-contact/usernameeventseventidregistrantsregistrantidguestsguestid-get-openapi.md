---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Get Guest Details
  description: Get Guest Details
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
  /{username}/campaigns/{campaign-id}/events/:
    get:
      summary: Get Campaign Events
      description: Get Campaign Events
      operationId: get-campaign-events
      x-api-path-slug: usernamecampaignscampaignidevents-get
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
      - Events
  /{username}/contacts:
    get:
      summary: List Contacts
      description: List Contacts
      operationId: list-contacts
      x-api-path-slug: usernamecontacts-get
      parameters:
      - in: query
        name: listid
        description: Specific list
      - in: query
        name: updatedsince
        description: Specified date
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
    post:
      summary: Add Contact
      description: Add Contact
      operationId: add-contact
      x-api-path-slug: usernamecontacts-post
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
      - Contact
  /{username}/contacts/{contact-id}:
    delete:
      summary: Opting-out Contact
      description: Opting-out Contact
      operationId: optingout-contact
      x-api-path-slug: usernamecontactscontactid-delete
      parameters:
      - in: path
        name: contact-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Opting-out
      - Contact
    get:
      summary: Get Contact
      description: Get Contact
      operationId: get-contact
      x-api-path-slug: usernamecontactscontactid-get
      parameters:
      - in: path
        name: contact-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Contact
    put:
      summary: Update Contact
      description: Update Contact
      operationId: update-contact
      x-api-path-slug: usernamecontactscontactid-put
      parameters:
      - in: path
        name: contact-id
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Contact
  /{username}/contacts/{contact-id}/events/:
    get:
      summary: Get Per-Contact Campaign Events
      description: Get Per-Contact Campaign Events
      operationId: get-percontact-campaign-events
      x-api-path-slug: usernamecontactscontactidevents-get
      parameters:
      - in: path
        name: contact-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Per-Contact
      - Campaign
      - Events
  /{username}/events:
    get:
      summary: List Events
      description: List Events
      operationId: list-events
      x-api-path-slug: usernameevents-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
    post:
      summary: Add Event
      description: Add Event
      operationId: add-event
      x-api-path-slug: usernameevents-post
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
      - Event
  /{username}/events/{event-id}:
    get:
      summary: Get Event
      description: Get Event
      operationId: get-event
      x-api-path-slug: usernameeventseventid-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Event
  /{username}/events/{event-id}/registrants:
    get:
      summary: List Registrants
      description: List Registrants
      operationId: list-registrants
      x-api-path-slug: usernameeventseventidregistrants-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Registrants
  /{username}/events/{event-id}/registrants/{registrant-id}:
    get:
      summary: Get Registrant
      description: Get Registrant
      operationId: get-registrant
      x-api-path-slug: usernameeventseventidregistrantsregistrantid-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Registrant
  /{username}/events/{event-id}/registrants/{registrant-id}/attendancestatus:
    get:
      summary: Get Attendance Status
      description: Get Attendance Status
      operationId: get-attendance-status
      x-api-path-slug: usernameeventseventidregistrantsregistrantidattendancestatus-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Attendance
      - Status
    put:
      summary: Update Attendance Status
      description: Update Attendance Status
      operationId: update-attendance-status
      x-api-path-slug: usernameeventseventidregistrantsregistrantidattendancestatus-put
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Attendance
      - Status
  /{username}/events/{event-id}/registrants/{registrant-id}/guests:
    get:
      summary: Get List of Guests
      description: Get List of Guests
      operationId: get-list-of-guests
      x-api-path-slug: usernameeventseventidregistrantsregistrantidguests-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Guests
  /{username}/events/{event-id}/registrants/{registrant-id}/guests/{guest-id}:
    get:
      summary: Get Guest Details
      description: Get Guest Details
      operationId: get-guest-details
      x-api-path-slug: usernameeventseventidregistrantsregistrantidguestsguestid-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: guest-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Guest
      - Details
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