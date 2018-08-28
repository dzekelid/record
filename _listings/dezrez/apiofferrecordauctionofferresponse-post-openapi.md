---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Record a auction offer Response
  version: 1.0.0
  description: Record a auction offer response.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/auction/{id}/recordbid:
    post:
      summary: Record auction bid details
      description: Record auction bid details.
      operationId: Auction_ReccordAuctionBidByidBydataContactDataContract
      x-api-path-slug: apiauctionidrecordbid-post
      parameters:
      - in: body
        name: dataContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Auction
      - Bid
      - Details
  /api/offer/recordoffer:
    post:
      summary: Record offer on a sale
      description: Record offer on a sale.
      operationId: Offer_RecordOfferByofferCommand
      x-api-path-slug: apiofferrecordoffer-post
      parameters:
      - in: body
        name: offerCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Offer
      - "On"
      - Sale
  /api/offer/progressnoteofinterest:
    post:
      summary: Record a note against on a offer
      description: Record a note against on a offer.
      operationId: Offer_ProgressNoteOfInterestByofferIdBydataContract
      x-api-path-slug: apiofferprogressnoteofinterest-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: offerId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Note
      - Against
      - "On"
      - Offer
  /api/offer/recordlettingoffer:
    post:
      summary: Record offer on a letting
      description: Record offer on a letting.
      operationId: Offer_RecordLettingOfferByofferCommand
      x-api-path-slug: apiofferrecordlettingoffer-post
      parameters:
      - in: body
        name: offerCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Offer
      - "On"
      - Letting
  /api/offer/recordofferresponse:
    post:
      summary: Record a sale/auction offer response
      description: Record a sale/auction offer response.
      operationId: Offer_RecordOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Sale
      - Auction
      - Offer
      - Response
  /api/offer/recordlettingofferresponse:
    post:
      summary: Record a letting offer response
      description: Record a letting offer response.
      operationId: Offer_RecordLettingOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordlettingofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Letting
      - Offer
      - Response
  /api/offer/recordauctionofferresponse:
    post:
      summary: Record a auction offer Response
      description: Record a auction offer response.
      operationId: Offer_RecordAuctionOfferResponseByrecordOfferResponseCommand
      x-api-path-slug: apiofferrecordauctionofferresponse-post
      parameters:
      - in: body
        name: recordOfferResponseCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Auction
      - Offer
      - Response
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