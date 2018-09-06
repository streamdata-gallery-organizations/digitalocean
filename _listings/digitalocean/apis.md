---
name: DigitalOcean
x-slug: digitalocean
description: DigitalOcean is a simple and fast cloud hosting service built for developers.
  Customers can create a cloud server in 55 seconds, and pricing plans start at only
  $5 per month for 512MB of RAM, 20GB SSD, 1 CPU, and 1TB Transfer. Featuring a 99.99%
  Uptime SLA, DigitalOcean has servers located in New York, San Francisco, and Amsterdam.
  The DigitalOcean control panel interface is simple and intuitive, which power users
  can replicate on a larger scale with the company&rsquo;s API. DigitalOcean uses
  KVM virtualization and additionally hosts a library of helpful walkthroughs and
  tutorials that cover server configuration and optimization.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
x-kinRank: "7"
x-alexaRank: "0"
tags: DigitalOcean
created: "2018-09-05"
modified: "2018-09-05"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/apis.md
specificationVersion: "0.14"
apis:
- name: DigitalOcean API-V2 - Get User Information
  x-api-slug: account-get
  description: Get [DigitalOcean](https://www.digitalocean.com/) account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/account-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/account-get-openapi.md
- name: DigitalOcean API-V2 - List all certificates
  x-api-slug: certificates-get
  description: "To list all of the certificates available on your account, send a
    GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with
    a certificates key. This will be set to an array of certificate objects, each
    of which will contain the standard certificate attributes:"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/certificates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/certificates-get-openapi.md
- name: DigitalOcean API-V2 - Create a new certificate
  x-api-slug: certificates-post
  description: To upload or create a new SSL certificate, send a POST request to /v2/certificates.
    When uploading a user-generated certificate, the private_key, leaf_certificate,
    and optionally the certificate_chain attributes should be provided. The type should
    be set to "custom". When generating a certificate using Let's Encrypt, the dns_names
    attribute must be provided, and the type should be set to "lets_encrypt".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/certificates-post-openapi.md
- name: DigitalOcean API-V2 - Retrieve an existing certificate
  x-api-slug: certificates892071a0bb9549bc80213afd67a210bf-get
  description: "To show information about an existing certificate, send a GET request
    to /v2/certificates/$CERTIFICATE_ID.\r\n\r\nThe response will be a JSON object
    with a certificate key."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/certificates892071a0bb9549bc80213afd67a210bf-get-openapi.md
- name: DigitalOcean API-V2 - Delete a certificate
  x-api-slug: certificates892071a0bb9549bc80213afd67a210bf-delete
  description: "To delete a specific certificate, send a DELETE request to /v2/certificates/$CERTIFICATE_ID.\r\n\r\nA
    status of 204 will be given. This indicates that the request was processed successfully,
    but that no response body is needed."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/certificates892071a0bb9549bc80213afd67a210bf-delete-openapi.md
- name: DigitalOcean API-V2 - List all Domains
  x-api-slug: domains-get
  description: "To retrieve a list of all of the domains in your account, send a GET
    request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called
    domains."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/domains-get-openapi.md
- name: DigitalOcean API-V2 - Listing Droplets by Tag
  x-api-slug: droplets-get
  description: "To list Droplets by a tag, send a GET request to /v2/droplets?tag_name=$TAG_NAME.\r\n\r\nThe
    response will match that of regular droplet listing request but will be filtered
    to only include the tagged Droplets."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/droplets-get-openapi.md
- name: DigitalOcean API-V2 - Create a new Droplet
  x-api-slug: droplets-post
  description: To create a new Droplet, send a POST request to /v2/droplets.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/droplets-post-openapi.md
- name: DigitalOcean API-V2 - Retrieve an existing Image by id
  x-api-slug: images63261821-get
  description: "To retrieve information about an image (public or private), send a
    GET request to /v2/images/$IMAGE_ID.\r\n\r\nThe response will be a JSON object
    with a key called image. The value of this will be an image object containing
    the standard image attributes:"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/images63261821-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/images63261821-get-openapi.md
- name: DigitalOcean API-V2 - Delete an Image
  x-api-slug: images63261821-delete
  description: "To delete an image, send a DELETE request to /v2/images/$IMAGE_ID.\r\n\r\nA
    status of 204 will be given. This indicates that the request was processed successfully,
    but that no response body is needed"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/images63261821-delete-openapi.md
- name: DigitalOcean API-V2 - List all Regions
  x-api-slug: regions-get
  description: "To list all of the regions that are available, send a GET request
    to /v2/regions.\r\n\r\nThe response will be a JSON object with a key called _regions_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/regions-get-openapi.md
- name: DigitalOcean API-V2 - List all Volume snapshots
  x-api-slug: snapshots-get
  description: To retrieve only snapshots based on volumes, include the resource_type
    query paramter set to volume, /v2/snapshots?resource_type=volume.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/snapshots-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/snapshots-get-openapi.md
- name: DigitalOcean API-V2 - List all Sizes
  x-api-slug: sizes-get
  description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
    response will be a JSON object with a key called _sizes_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/sizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/sizes-get-openapi.md
- name: DigitalOcean API-V2 - List all Keys
  x-api-slug: accountkeys-get
  description: "To list all of the keys in your account, send a GET request to /v2/account/keys.\r\n\r\nThe
    response will be a JSON object with a key set to _ssh_keys_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/accountkeys-get-openapi.md
- name: DigitalOcean API-V2 - Create a new Key
  x-api-slug: accountkeys-post
  description: "To add a new SSH public key to your DigitalOcean account, send a POST
    request to /v2/account/keys. Set the \"name\" attribute to the name you wish to
    use and the \"public_key\" attribute to a string of the full public key you are
    adding.\n\nThe response body will be a JSON object with a key set to ssh_key.
    The value will be the complete generated key object. This will have the standard
    key attributes:\n\nName\tType\tDescription\nid\tinteger\tThis is a unique identification
    number for the key. This can be used to reference a specific SSH key when you
    wish to embed a key into a Droplet.\nfingerprint\tstring\tThis attribute contains
    the fingerprint value that is generated from the public key. This is a unique
    identifier that will differentiate it from other keys using a format that SSH
    recognizes.\npublic_key\tstring\tThis attribute contains the entire public key
    string that was uploaded. This is what is embedded into the root user's authorized_keys
    file if you choose to include this SSH key during Droplet creation.\nname\tstring\tThis
    is the human-readable display name for the given SSH key. This is used to easily
    identify the SSH keys when they are displayed."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/accountkeys-post-openapi.md
- name: DigitalOcean API-V2 - Retrieve an existing Key
  x-api-slug: accountkeys22162952-get
  description: "To show information about a key, send a GET request to /v2/account/keys/$KEY_ID
    or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nThe response will be a JSON object
    with a key called _ssh_key_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/accountkeys22162952-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/accountkeys22162952-get-openapi.md
- name: DigitalOcean API-V2 - Update a Key
  x-api-slug: accountkeys22162952-put
  description: To update the name of an SSH key, send a PUT request to either /v2/account/keys/$SSH_KEY_ID
    or /v2/account/keys/$SSH_KEY_FINGERPRINT. Set the "name" attribute to the new
    name you want to use.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/accountkeys22162952-put-openapi.md
- name: DigitalOcean API-V2 - Destroy a Key
  x-api-slug: accountkeys22162952-delete
  description: "To destroy a public SSH key that you have in your account, send a
    DELETE request to /v2/account/keys/$KEY_ID or /v2/account/keys/$KEY_FINGERPRINT.\r\n\r\nA
    204 status will be returned, indicating that the action was successful and that
    the response body is empty."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/accountkeys22162952-delete-openapi.md
- name: DigitalOcean API-V2 - List all Tags
  x-api-slug: tags-get
  description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
    response will be a JSON object with a key called _tags_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/tags-get-openapi.md
- name: DigitalOcean API-V2 - Create a new Tag
  x-api-slug: tags-post
  description: "To create a Tag you can send a POST request to /v2/tags with a name
    attribute.\r\n\r\nThe response will be a JSON object with a key called _tag_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/tags-post-openapi.md
- name: DigitalOcean API-V2 - Tag a Resource
  x-api-slug: tagspostmandotagresources-post
  description: "Resources can be tagged by sending a POST request to /v2/tags/$TAG_NAME/resources
    with an array of json objects containing resource_id and resource_type attributes.\r\n\r\nCurrently
    only tagging of Droplets is supported. resource_id is expected to be the Droplet's
    id attribute as a string, and resource_type is expected to be the string droplet."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/digitalocean/master/_listings/digitalocean/tagspostmandotagresources-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://digital.river.api.gallery.streamdata.io
- type: x-api-stack
  url: http://digitalocean.stack.network
- type: x-base
  url: https://api.digitalocean.com/
- type: x-blog
  url: https://www.digitalocean.com/company/blog/
- type: x-blog-rss
  url: https://www.digitalocean.com/company/blog/feed.xml
- type: x-command-line-interface
  url: https://github.com/digitalocean/doctl
- type: x-developer
  url: https://developers.digitalocean.com/
- type: x-github
  url: https://github.com/digitalocean
- type: x-twitter
  url: https://twitter.com/digitalocean
- type: x-website
  url: https://www.digitalocean.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---