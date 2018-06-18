---
name: Infermedica
x-slug: infermedica
description: At Infermedica we believe in people. Every team member brings unique
  skills, talent and knowledge. Together we solve the most complex healthcare problems.
  Infermedica improves the diagnostic process using the most advanced reasoning technology
  for preliminary medical diagnosis.White-labelled enterprise platform (web, mobile,
  chatbot or voice-enabled applications) for symptom checking, patient triage and
  clinical decision support. Open developer portal that allows to easily integrate
  our diagnostic engine into 3rd party software.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/infermedica-logo.jpeg
x-kinRank: "7"
x-alexaRank: "0"
tags: Conditions
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/infermedica/apis.md
specificationVersion: "0.14"
apis:
- name: Infermedica Get Conditions
  x-api-slug: infermedica
  description: Returns a list of all available conditions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/infermedica-logo.jpeg
  humanURL: http://infermedica.com
  baseURL: https://api.infermedica.com//v1//conditions
  tags: Healthcare,Conditions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/infermedica/conditions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/infermedica/conditions-get-openapi.md
- name: Infermedica Get Conditions
  x-api-slug: infermedica
  description: Returns details of a single condition specified by id parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/infermedica-logo.jpeg
  humanURL: http://infermedica.com
  baseURL: https://api.infermedica.com//v1//conditions/{id}
  tags: Healthcare,Conditions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/infermedica/conditionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/infermedica/conditionsid-get-openapi.md
- name: Infermedica
  x-api-slug: infermedica
  description: At Infermedica we believe in people. Every team member brings unique
    skills, talent and knowledge. Together we solve the most complex healthcare problems.
    Infermedica improves the diagnostic process using the most advanced reasoning
    technology for preliminary medical diagnosis.White-labelled enterprise platform
    (web, mobile, chatbot or voice-enabled applications) for symptom checking, patient
    triage and clinical decision support. Open developer portal that allows to easily
    integrate our diagnostic engine into 3rd party software.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/infermedica-logo.jpeg
  humanURL: http://infermedica.com
  baseURL: https://api.infermedica.com//v1
  tags: Conditions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/conditions/master/_listings/infermedica/openapi.md
x-common:
- type: x-blog
  url: https://blog.infermedica.com/
- type: x-blog-rss
  url: https://blog.infermedica.com/rss/
- type: x-curated-source
  url: https://developer.infermedica.com/
- type: x-developer
  url: http://developer.infermedica.com
- type: x-github
  url: https://github.com/infermedica
- type: x-status
  url: http://status.infermedica.com/
- type: x-twitter
  url: https://twitter.com/infermedica
- type: x-website
  url: http://infermedica.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---