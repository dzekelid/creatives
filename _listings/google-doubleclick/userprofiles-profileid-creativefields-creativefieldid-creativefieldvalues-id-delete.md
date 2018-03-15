---
swagger: "2.0"
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/creativeFields/{creativeFieldId}/creativeFieldValues/{id}:
    delete:
      summary: Delete Creative Field Value
      description: Deletes an existing creative field value
      operationId: dfareporting.creativeFieldValues.delete
      parameters:
      - in: path
        name: creativeFieldId
        description: Creative field ID for this creative field value
      - in: path
        name: id
        description: Creative Field Value ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - advertising
      - creative field
definitions: []
x-collection-name: Google Doubleclick
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