---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean Update a Key
  description: To update the name of an SSH key, send a PUT request to either /v2/account/keys/$SSH_KEY_ID
    or /v2/account/keys/$SSH_KEY_FINGERPRINT. Set the "name" attribute to the new
    name you want to use.
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
    delete:
      summary: Delete an Image
      description: "To delete an image, send a DELETE request to /v2/images/$IMAGE_ID.\r\n\r\nA
        status of 204 will be given. This indicates that the request was processed
        successfully, but that no response body is needed"
      operationId: Images63261821Delete
      x-api-path-slug: images63261821-delete
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Image
  /regions:
    get:
      summary: List all Regions
      description: "To list all of the regions that are available, send a GET request
        to /v2/regions.\r\n\r\nThe response will be a JSON object with a key called
        _regions_."
      operationId: RegionsGet
      x-api-path-slug: regions-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Regions
  /snapshots:
    get:
      summary: List all Volume snapshots
      description: To retrieve only snapshots based on volumes, include the resource_type
        query paramter set to volume, /v2/snapshots?resource_type=volume.
      operationId: SnapshotsGet3
      x-api-path-slug: snapshots-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: resource_type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Volume
      - Snapshots
  /sizes:
    get:
      summary: List all Sizes
      description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
        response will be a JSON object with a key called _sizes_."
      operationId: SizesGet
      x-api-path-slug: sizes-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Sizes
  /account/keys:
    get:
      summary: List all Keys
      description: "To list all of the keys in your account, send a GET request to
        /v2/account/keys.\r\n\r\nThe response will be a JSON object with a key set
        to _ssh_keys_."
      operationId: AccountKeysGet
      x-api-path-slug: accountkeys-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Keys
    post:
      summary: Create a new Key
      description: "To add a new SSH public key to your DigitalOcean account, send
        a POST request to /v2/account/keys. Set the \"name\" attribute to the name
        you wish to use and the \"public_key\" attribute to a string of the full public
        key you are adding.\n\nThe response body will be a JSON object with a key
        set to ssh_key. The value will be the complete generated key object. This
        will have the standard key attributes:\n\nName\tType\tDescription\nid\tinteger\tThis
        is a unique identification number for the key. This can be used to reference
        a specific SSH key when you wish to embed a key into a Droplet.\nfingerprint\tstring\tThis
        attribute contains the fingerprint value that is generated from the public
        key. This is a unique identifier that will differentiate it from other keys
        using a format that SSH recognizes.\npublic_key\tstring\tThis attribute contains
        the entire public key string that was uploaded. This is what is embedded into
        the root user's authorized_keys file if you choose to include this SSH key
        during Droplet creation.\nname\tstring\tThis is the human-readable display
        name for the given SSH key. This is used to easily identify the SSH keys when
        they are displayed."
      operationId: AccountKeysPost
      x-api-path-slug: accountkeys-post
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
      - Key
  /account/keys/22162952:
    get:
      summary: Retrieve an existing Key
      description: "To show information about a key, send a GET request to /v2/account/keys/$KEY_ID
        or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nThe response will be a JSON object
        with a key called _ssh_key_."
      operationId: AccountKeys22162952Get
      x-api-path-slug: accountkeys22162952-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Existing
      - Key
    put:
      summary: Update a Key
      description: To update the name of an SSH key, send a PUT request to either
        /v2/account/keys/$SSH_KEY_ID or /v2/account/keys/$SSH_KEY_FINGERPRINT. Set
        the "name" attribute to the new name you want to use.
      operationId: AccountKeys22162952Put
      x-api-path-slug: accountkeys22162952-put
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
      - Key
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