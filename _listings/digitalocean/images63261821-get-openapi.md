---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean Retrieve an existing Image by id
  description: "To retrieve information about an image (public or private), send a
    GET request to /v2/images/$IMAGE_ID.\r\n\r\nThe response will be a JSON object
    with a key called image. The value of this will be an image object containing
    the standard image attributes:"
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
    post:
      summary: Create a new certificate
      description: To upload or create a new SSL certificate, send a POST request
        to /v2/certificates. When uploading a user-generated certificate, the private_key,
        leaf_certificate, and optionally the certificate_chain attributes should be
        provided. The type should be set to "custom". When generating a certificate
        using Let's Encrypt, the dns_names attribute must be provided, and the type
        should be set to "lets_encrypt".
      operationId: CertificatesPost
      x-api-path-slug: certificates-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - New
      - Certificate
  /certificates/892071a0-bb95-49bc-8021-3afd67a210bf:
    get:
      summary: Retrieve an existing certificate
      description: "To show information about an existing certificate, send a GET
        request to /v2/certificates/$CERTIFICATE_ID.\r\n\r\nThe response will be a
        JSON object with a certificate key."
      operationId: Certificates892071a0Bb9549bc80213afd67a210bfGet
      x-api-path-slug: certificates892071a0bb9549bc80213afd67a210bf-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Existing
      - Certificate
    delete:
      summary: Delete a certificate
      description: "To delete a specific certificate, send a DELETE request to /v2/certificates/$CERTIFICATE_ID.\r\n\r\nA
        status of 204 will be given. This indicates that the request was processed
        successfully, but that no response body is needed."
      operationId: Certificates892071a0Bb9549bc80213afd67a210bfDelete
      x-api-path-slug: certificates892071a0bb9549bc80213afd67a210bf-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Certificate
  /domains:
    get:
      summary: List all Domains
      description: "To retrieve a list of all of the domains in your account, send
        a GET request to /v2/domains.\r\n\r\nThe response will be a JSON object with
        a key called domains."
      operationId: DomainsGet
      x-api-path-slug: domains-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Domains
  /droplets:
    get:
      summary: Listing Droplets by Tag
      description: "To list Droplets by a tag, send a GET request to /v2/droplets?tag_name=$TAG_NAME.\r\n\r\nThe
        response will match that of regular droplet listing request but will be filtered
        to only include the tagged Droplets."
      operationId: DropletsGet2
      x-api-path-slug: droplets-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: tag_name
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Droplets
      - By
      - Tag
    post:
      summary: Create a new Droplet
      description: To create a new Droplet, send a POST request to /v2/droplets.
      operationId: DropletsPost
      x-api-path-slug: droplets-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - New
      - Droplet
  /images/63261821:
    get:
      summary: Retrieve an existing Image by id
      description: "To retrieve information about an image (public or private), send
        a GET request to /v2/images/$IMAGE_ID.\r\n\r\nThe response will be a JSON
        object with a key called image. The value of this will be an image object
        containing the standard image attributes:"
      operationId: Images63261821Get
      x-api-path-slug: images63261821-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Existing
      - Image
      - By
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