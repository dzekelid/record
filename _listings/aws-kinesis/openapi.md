swagger: "2.0"
x-collection-name: AWS Kinesis
x-complete: 1
info:
  title: AWS Kinesis Firehose API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutRecord:
    get:
      summary: Put Record
      description: writes a single data record into an Amazon Kinesis Firehose delivery
        stream.
      operationId: PutRecord
      x-api-path-slug: actionputrecord-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: Record
        description: The record
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records
  /?Action=PutRecordBatch:
    get:
      summary: Put Record Batch
      description: |-
        writes multiple data records into a delivery stream in a single call, which can
                 achieve higher throughput per producer than when writing single records.
      operationId: PutRecordBatch
      x-api-path-slug: actionputrecordbatch-get
      parameters:
      - in: query
        name: DeliveryStreamName
        description: The name of the delivery stream
        type: string
      - in: query
        name: Records
        description: One or more records
        type: string
      responses:
        200:
          description: OK
      tags:
      - Records