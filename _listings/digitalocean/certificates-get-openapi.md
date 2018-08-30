---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean List all certificates
  description: "To list all of the certificates available on your account, send a
    GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with
    a certificates key. This will be set to an array of certificate objects, each
    of which will contain the standard certificate attributes:"
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account:
    get:
      summary: Get User Information
      description: Get [DigitalOcean](https://www.digitalocean.com/) account
      operationId: AccountGet
      x-api-path-slug: account-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - User
      - Information
  /certificates:
    get:
      summary: List all certificates
      description: "To list all of the certificates available on your account, send
        a GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object
        with a certificates key. This will be set to an array of certificate objects,
        each of which will contain the standard certificate attributes:"
      operationId: CertificatesGet
      x-api-path-slug: certificates-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Certificates
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