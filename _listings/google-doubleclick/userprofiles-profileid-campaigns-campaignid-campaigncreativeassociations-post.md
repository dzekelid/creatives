---
swagger: "2.0"
info:
  title: Google Doubleclick API Add Campaign Creative
  version: 1.0.0
  description: Associates a creative with the specified campaign. This method creates
    a default ad with dimensions matching the creative in the campaign if such a default
    ad does not exist already.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/campaigns/{campaignId}/campaignCreativeAssociations:
    post:
      summary: Add Campaign Creative
      description: Associates a creative with the specified campaign
      operationId: dfareporting.campaignCreativeAssociations.insert
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: campaignId
        description: Campaign ID in this association
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - advertising
      - campaign creatives
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