---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Get Recording
  description: Returns one of several representations:nWithout an extension, or with
    a .wav, a binary WAV audio file is returnednwith mime-type audio/x-wav.nAppending
    .mp3 to the URI returns a binary MP3 audio file with mime-typentype audio/mpeg.nAppending
    .xml to the URI returns a XML representation.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Calls/{CallSid}/Recordings.{format}:
    get:
      summary: Get Recordings
      description: Returns a list of Recording resource representations, each representing
        anrecording generated during the course of a phone call.n
      operationId: returns-a-list-of-recording-resource-representations-each-representing-arecording-generated-during-t
      x-api-path-slug: accountsaccountsidcallscallsidrecordings-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CallSid
        description: A 34 character string that uniquely identifies the call
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Recordings
  /Accounts/{AccountSid}/Recordings:
    get:
      summary: Get Recordings
      description: Returns a list of Recording resource representations, each representing
        anrecording generated during the course of a phone call.n
      operationId: returns-a-list-of-recording-resource-representations-each-representing-arecording-generated-during-t
      x-api-path-slug: accountsaccountsidrecordings-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Recordings
  /Accounts/{AccountSid}/Recordings/{RecordingSid}:
    delete:
      summary: Delete Recording
      description: Deletes a recording  from your account.
      operationId: deletes-a-recording--from-your-account
      x-api-path-slug: accountsaccountsidrecordingsrecordingsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: RecordingSid
        description: A 34 character string that uniquely identifies the recording
      responses:
        200:
          description: OK
      tags:
      - Recordings
    get:
      summary: Get Recording
      description: Returns one of several representations:nWithout an extension, or
        with a .wav, a binary WAV audio file is returnednwith mime-type audio/x-wav.nAppending
        .mp3 to the URI returns a binary MP3 audio file with mime-typentype audio/mpeg.nAppending
        .xml to the URI returns a XML representation.n
      operationId: returns-one-of-several-representationswithout-an-extension-or-with-a-wav-a-binary-wav-audio-file-is-
      x-api-path-slug: accountsaccountsidrecordingsrecordingsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: RecordingSid
        description: A 34 character string that uniquely identifies the recording
      responses:
        200:
          description: OK
      tags:
      - Recordings
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