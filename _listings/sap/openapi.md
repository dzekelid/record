swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
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