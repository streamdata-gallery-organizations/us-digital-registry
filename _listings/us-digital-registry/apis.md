---
name: US Digital Registry
x-slug: us-digital-registry
description: Whether for access to emergency, financial or education public services,
  users need to trust they are engaging with official U.S. government digital accounts.
  The U.S. Digital Registry serves as the authoritative resource for agencies, citizens
  and developers to confirm the official status of social media and public-facing
  collaboration accounts, mobile apps and mobile websites, and help prevent exploitation
  from unofficial sources, phishing scams or malicious entities.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
x-kinRank: "9"
x-alexaRank: "0"
tags: US Digital Registry
created: "2018-08-31"
modified: "2018-08-31"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/apis.md
specificationVersion: "0.14"
apis:
- name: U.S. Digital Registry Agency API - Agencies
  x-api-slug: agencies-json-get
  description: This lists all active agencies in the system. These agencies can be
    used to query for social media accounts, mobile products, and galleries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/agencies-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/agencies-json-get-openapi.md
- name: U.S. Digital Registry Agency API - Agency
  x-api-slug: agenciesid-json-get
  description: This returns an agency based on an ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/agenciesid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/agenciesid-json-get-openapi.md
- name: U.S. Digital Registry Mobile App API - Mobile App Token
  x-api-slug: mobile-appstokeninput-json-get
  description: This returns tokens representing agencies, tags, and a basic text search
    token for the purpose of building search dialogs
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1/
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/mobile-appstokeninput-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/mobile-appstokeninput-json-get-openapi.md
- name: U.S. Digital Registry Mobile App API - Mobile Apps
  x-api-slug: mobile-apps-json-get
  description: This lists all active mobile apps.  It accepts parameters to perform
    basic search as well as searching by tag and agency.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1/
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/mobile-apps-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/mobile-apps-json-get-openapi.md
- name: U.S. Digital Registry Mobile App API - Mobile App
  x-api-slug: mobile-appsid-json-get
  description: This returns an mobile app based on an ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1/
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/mobile-appsid-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/mobile-appsid-json-get-openapi.md
- name: U.S. Digital Registry Social Media API - Social Media Verify
  x-api-slug: social-mediaverify-json-get
  description: This returns an agency based on an URL. If not found, it will return
    a 404
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/social-mediaverify-json-get-openapi.md
- name: U.S. Digital Registry Social Media API - Social Media Services
  x-api-slug: social-mediaservices-json-get
  description: This returns a list of services along with the number of accounts registered
    with them
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/social-mediaservices-json-get-openapi.md
- name: U.S. Digital Registry Social Media API - Social Media Token
  x-api-slug: social-mediatokeninput-json-get
  description: This returns tokens representing services, agencies, tags, and a basic
    text search token for the purpose of building search dialogs
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/social-mediatokeninput-json-get-openapi.md
- name: U.S. Digital Registry Social Media API - Social Media
  x-api-slug: social-media-json-get
  description: This lists all active accounts. It accepts parameters to perform basic
    search as well as search by service, agency, or tags.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/social-media-json-get-openapi.md
- name: U.S. Digital Registry Social Media API - Social Media
  x-api-slug: social-mediaid-json-get
  description: This returns an agency based on an ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/social-mediaid-json-get-openapi.md
- name: U.S. Digital Registry Tag API - Tag Types
  x-api-slug: tagstypes-json-get
  description: This returns a tag based on an ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1/
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/tagstypes-json-get-openapi.md
- name: U.S. Digital Registry Tag API - Tags
  x-api-slug: tags-json-get
  description: This lists all tags.  It accepts parameters to perform basic search.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1/
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/tags-json-get-openapi.md
- name: U.S. Digital Registry Tag API - Tag
  x-api-slug: tagsid-json-get
  description: This returns a tag based on an ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/digital-gov-logo.jpeg
  humanURL: https://usdigitalregistry.digitalgov.gov
  baseURL: https://usdigitalregistry.digitalgov.gov//api/v1/
  tags: Federal Government   GSA, Stack Network, General Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/us-digital-registry/master/_listings/us-digital-registry/tagsid-json-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://tyk.api.gallery.streamdata.io
- type: x-api-stack
  url: http://u.s..digital.registry.stack.network
- type: x-website
  url: https://usdigitalregistry.digitalgov.gov
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---