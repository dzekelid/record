---
swagger: "2.0"
x-collection-name: AWS X-Ray
x-complete: 0
info:
  title: AWS X-Ray API Put Telemetry Records
  version: 1.0.0
  description: Used by the AWS X-Ray daemon to upload telemetry.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutTelemetryRecords:
    get:
      summary: Put Telemetry Records
      description: Used by the AWS X-Ray daemon to upload telemetry.
      operationId: putTelemetryRecords
      x-api-path-slug: actionputtelemetryrecords-get
      parameters:
      - in: query
        name: EC2InstanceId
        type: string
      - in: query
        name: Hostname
        type: string
      - in: query
        name: ResourceARN
        type: string
      - in: query
        name: TelemetryRecords
        type: string
      responses:
        200:
          description: OK
      tags:
      - Telemetry Records
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