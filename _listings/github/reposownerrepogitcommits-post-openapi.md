---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Add Repos Owner Repo Git Commits
  description: Create a Commit.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gitignore/templates:
    get:
      summary: Get Gitignore Templates
      description: |-
        Listing available templates.
        List all templates available to pass as an option when creating a repository.
      operationId: listing-available-templateslist-all-templates-available-to-pass-as-an-option-when-creating-a-reposit
      x-api-path-slug: gitignoretemplates-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      responses:
        200:
          description: OK
      tags:
      - Gitignore
      - Templates
  /gitignore/templates/{language}:
    get:
      summary: Get Gitignore Templates Language
      description: Get a single template.
      operationId: get-a-single-template
      x-api-path-slug: gitignoretemplateslanguage-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: language
      responses:
        200:
          description: OK
      tags:
      - Gitignore
      - Templates
      - Language
  /repos/{owner}/{repo}/git/blobs:
    post:
      summary: Add Repos Owner Repo Git Blobs
      description: Create a Blob.
      operationId: create-a-blob
      x-api-path-slug: reposownerrepogitblobs-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Blobs
  /repos/{owner}/{repo}/git/blobs/{shaCode}:
    get:
      summary: Get Repos Owner Repo Git Blobs Shacode
      description: |-
        Get a Blob.
        Since blobs can be any arbitrary binary data, the input and responses for
        the blob API takes an encoding parameter that can be either utf-8 or
        base64. If your data cannot be losslessly sent as a UTF-8 string, you can
        base64 encode it.
      operationId: get-a-blobsince-blobs-can-be-any-arbitrary-binary-data-the-input-and-responses-forthe-blob-api-takes
      x-api-path-slug: reposownerrepogitblobsshacode-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      - in: path
        name: shaCode
        description: SHA-1 code
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Blobs
      - Shacode
  /repos/{owner}/{repo}/git/commits:
    post:
      summary: Add Repos Owner Repo Git Commits
      description: Create a Commit.
      operationId: create-a-commit
      x-api-path-slug: reposownerrepogitcommits-post
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Commits
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