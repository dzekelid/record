---
swagger: "2.0"
x-collection-name: Backupify
x-complete: 0
info:
  title: Backupify Retrieve a specific record by id for the specified endpoint and
    backup_instance
  description: You can only retrieve records for endpoints of backup_instances you
    have access to
  version: 1.0.0
host: api.backupify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/backup_instances/{backup_instance_id}/endpoints/{endpoint_name}/records/{record_id}:
    get:
      summary: Retrieve a specific record by id for the specified endpoint and backup_instance
      description: You can only retrieve records for endpoints of backup_instances
        you have access to
      operationId: getV1BackupInstancesBackupInstanceEndpointsEndpointNameRecordsRecord
      x-api-path-slug: v1backup-instancesbackup-instance-idendpointsendpoint-namerecordsrecord-id-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      - in: path
        name: endpoint_name
        description: The name of the endpoint to retrieve the record from
      - in: path
        name: record_id
        description: The id of the endpoint record to retrieve
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Endpoints
      - Endpoint
      - Name
      - Records
      - Record
      - Id
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