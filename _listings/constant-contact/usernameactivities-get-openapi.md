---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact List Activities
  description: List Activities
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