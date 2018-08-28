---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Records an event on the role representing a neg being in contact for
    an owner
  version: 1.0.0
  description: Records an event on the role representing a neg being in contact for
    an owner.
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
  /api/property/recordvaluation:
    post:
      summary: A command driven endpoint to Record a Valuation.
      description: A command driven endpoint to record a valuation..
      operationId: Property_RecordValuationByrecordValuationData
      x-api-path-slug: apipropertyrecordvaluation-post
      parameters:
      - in: body
        name: recordValuationData
        description: A wrapper for the various data contracts needed
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - A
      - Command
      - Driven
      - Endpoint
      - To
      - Record
      - Valuation
  /api/stats/RecordVisit/{pageType}/{entityId}:
    post:
      summary: Record and timestamp a visit to a 'page' on Rezi.
      description: Record and timestamp a visit to a 'page' on rezi..
      operationId: Stats_RecordVisitBypageTypeByentityIdByroleId
      x-api-path-slug: apistatsrecordvisitpagetypeentityid-post
      parameters:
      - in: path
        name: entityId
        description: The relative entitiyId e
      - in: path
        name: pageType
        description: GroupHub, PropertyHub, MarketingHub, PersonHub, SalesProgressionHub
          or PreTenancyHub
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
        description: The RoleId if applicable (can be null if omitted)
      responses:
        200:
          description: OK
      tags:
      - Record
      - Timestamp
      - Visit
      - To
      - Page
      - "On"
      - Rezi
  /api/valuation/{valuationId}/recordfeedback:
    post:
      summary: Record and edit the feedback against a Valuation.
      description: Record and edit the feedback against a valuation..
      operationId: Valuation_RecordFeedbackByvaluationIdByfeedbackByimpressionByfeedbackDateBynegIds
      x-api-path-slug: apivaluationvaluationidrecordfeedback-post
      parameters:
      - in: query
        name: feedback
        description: feedback text
      - in: query
        name: feedbackDate
      - in: query
        name: impression
      - in: query
        name: negIds
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: valuationId
        description: valuation id
      responses:
        200:
          description: OK
      tags:
      - Record
      - Edit
      - Feedback
      - Against
      - Valuation
  /api/valuation/{valuationId}/feedbacknotified:
    post:
      summary: Record that the feedback for a Valuation was notified to the vendor.
      description: Record that the feedback for a valuation was notified to the vendor..
      operationId: Valuation_FeedbackNotifiedByvaluationIdBynotifiedDateBynegotiatorIdsByvendorNotified
      x-api-path-slug: apivaluationvaluationidfeedbacknotified-post
      parameters:
      - in: query
        name: negotiatorIds
        description: The negotiator(s) who notified the vendor
      - in: query
        name: notifiedDate
        description: The date the vendor was notified
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: valuationId
        description: valuation id
      - in: query
        name: vendorNotified
        description: Whether or not the vendor has been notified
      responses:
        200:
          description: OK
      tags:
      - Record
      - That
      - Feedbacka
      - Valuation
      - Was
      - Notified
      - To
      - Vendor
  /api/viewing/{id}/recordfeedback:
    post:
      summary: Record the feedback against a Viewing.
      description: Record the feedback against a viewing..
      operationId: Viewing_RecordFeedbackByidBycommand
      x-api-path-slug: apiviewingidrecordfeedback-post
      parameters:
      - in: body
        name: command
        description: Feedback details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Viewing id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Record
      - Feedback
      - Against
      - Viewing
  /api/viewing/{viewingFeedbackId}/feedbacknotified:
    post:
      summary: Record that the feedback for a Viewing was notified to the vendor.
      description: Record that the feedback for a viewing was notified to the vendor..
      operationId: Viewing_FeedbackNotifiedByviewingFeedbackIdBytypeBynotifiedDateBynegIds
      x-api-path-slug: apiviewingviewingfeedbackidfeedbacknotified-post
      parameters:
      - in: query
        name: negIds
      - in: query
        name: notifiedDate
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: type
        description: Task type for how vendor was communicated e
      - in: path
        name: viewingFeedbackId
        description: viewing feedback id
      responses:
        200:
          description: OK
      tags:
      - Record
      - That
      - Feedbacka
      - Viewing
      - Was
      - Notified
      - To
      - Vendor
  /api/event/recordenquiry:
    post:
      summary: Records an event on the role representing a neg being in contact with
        a person
      description: Records an event on the role representing a neg being in contact
        with a person.
      operationId: Event_RecordEnquiryByrecordEnquiryDataContract
      x-api-path-slug: apieventrecordenquiry-post
      parameters:
      - in: body
        name: recordEnquiryDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contact
      - Person
  /api/event/recordownercontact:
    post:
      summary: Records an event on the role representing a neg being in contact for
        an owner
      description: Records an event on the role representing a neg being in contact
        for an owner.
      operationId: Event_RecordOwnerContactByrecordOwnerContactDataContract
      x-api-path-slug: apieventrecordownercontact-post
      parameters:
      - in: body
        name: recordOwnerContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contactan
      - Owner
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