---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Intelligent Mapping Insert an individual feature into a collection.
  description: |-
    Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
    The GeoJSON id included in the url must match the top level id member of the feature provided.
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/collections/{collectionName}/features:
    post:
      summary: Insert an individual feature into a collection.
      description: |-
        Insert a new feature into the the named collection. The GeoJSON id is used to identify the feature.
        The GeoJSON id included in the url must match the top level id member of the feature provided.
      operationId: insert-a-new-feature-into-the-the-named-collection-the-geojson-id-is-used-to-identify-the-featurethe
      x-api-path-slug: v1collectionscollectionnamefeatures-post
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Individual
      - Feature
      - Into
      - Collection
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