---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Adds a record to the order history
  description: "Adds a record to the history of an order.   \nThe order number is
    sent in the message body of the Order Created event.  \nThe login user must be
    from the additive manufacturing supplier."
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/{orderNumber}/history:
    post:
      summary: Adds a record to the order history
      description: "Adds a record to the history of an order.   \nThe order number
        is sent in the message body of the Order Created event.  \nThe login user
        must be from the additive manufacturing supplier."
      operationId: adds-a-record-to-the-history-of-an-order---the-order-number-is-sent-in-the-message-body-of-the-order
      x-api-path-slug: ordersordernumberhistory-post
      parameters:
      - in: body
        name: OrderItemRequest
        description: A request about an order
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderNumber
        description: An order number
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Record
      - To
      - Order
      - History
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