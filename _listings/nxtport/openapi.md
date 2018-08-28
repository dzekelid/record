swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/deliveries:
    post:
      summary: Record delivery
      description: When the driver has delivered the container, a request should be
        sent to the server to record (create) the delivery. Note that a delivery is
        associated with a PickupRight, because the driver who gets a PickupRight,
        will automatically get a right to deliver the container. For that reason,
        the PickupRight must be reported.
      operationId: postApiV1Deliveries
      x-api-path-slug: apiv1deliveries-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - Record
      - Delivery