---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Get Repos Owner Repo Git Trees Shacode
  description: Get a Tree.
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
  /repos/{owner}/{repo}/git/commits/{shaCode}:
    get:
      summary: Get Repos Owner Repo Git Commits Shacode
      description: Get a Commit.
      operationId: get-a-commit
      x-api-path-slug: reposownerrepogitcommitsshacode-get
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
      - Commits
      - Shacode
  /repos/{owner}/{repo}/git/refs:
    get:
      summary: Get Repos Owner Repo Git Refs
      description: Get all References
      operationId: get-all-references
      x-api-path-slug: reposownerrepogitrefs-get
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
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Refs
    post:
      summary: Add Repos Owner Repo Git Refs
      description: Create a Reference
      operationId: create-a-reference
      x-api-path-slug: reposownerrepogitrefs-post
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
      - Refs
  /repos/{owner}/{repo}/git/refs/{ref}:
    delete:
      summary: Delete Repos Owner Repo Git Refs Ref
      description: "Delete a Reference\nExample: Deleting a branch: DELETE /repos/octocat/Hello-World/git/refs/heads/feature-a
        \nExample: Deleting a tag:        DELETE /repos/octocat/Hello-World/git/refs/tags/v1.0"
      operationId: delete-a-referenceexample-deleting-a-branch-delete-reposoctocathelloworldgitrefsheadsfeaturea-exampl
      x-api-path-slug: reposownerrepogitrefsref-delete
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
        name: ref
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
      - Refs
      - Ref
    get:
      summary: Get Repos Owner Repo Git Refs Ref
      description: Get a Reference
      operationId: get-a-reference
      x-api-path-slug: reposownerrepogitrefsref-get
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
        name: ref
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
      - Refs
      - Ref
    patch:
      summary: Patch Repos Owner Repo Git Refs Ref
      description: Update a Reference
      operationId: update-a-reference
      x-api-path-slug: reposownerrepogitrefsref-patch
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
        name: ref
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
      - Refs
      - Ref
  /repos/{owner}/{repo}/git/tags:
    post:
      summary: Add Repos Owner Repo Git Tags
      description: |-
        Create a Tag Object.
        Note that creating a tag object does not create the reference that makes a
        tag in Git. If you want to create an annotated tag in Git, you have to do
        this call to create the tag object, and then create the refs/tags/[tag]
        reference. If you want to create a lightweight tag, you only have to create
        the tag reference - this call would be unnecessary.
      operationId: create-a-tag-objectnote-that-creating-a-tag-object-does-not-create-the-reference-that-makes-atag-in-
      x-api-path-slug: reposownerrepogittags-post
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
      - Tags
  /repos/{owner}/{repo}/git/tags/{shaCode}:
    get:
      summary: Get Repos Owner Repo Git Tags Shacode
      description: Get a Tag.
      operationId: get-a-tag
      x-api-path-slug: reposownerrepogittagsshacode-get
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
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Tags
      - Shacode
  /repos/{owner}/{repo}/git/trees:
    post:
      summary: Add Repos Owner Repo Git Trees
      description: |-
        Create a Tree.
        The tree creation API will take nested entries as well. If both a tree and
        a nested path modifying that tree are specified, it will overwrite the
        contents of that tree with the new path contents and write a new tree out.
      operationId: create-a-treethe-tree-creation-api-will-take-nested-entries-as-well-if-both-a-tree-anda-nested-path-
      x-api-path-slug: reposownerrepogittrees-post
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
      - Trees
  /repos/{owner}/{repo}/git/trees/{shaCode}:
    get:
      summary: Get Repos Owner Repo Git Trees Shacode
      description: Get a Tree.
      operationId: get-a-tree
      x-api-path-slug: reposownerrepogittreesshacode-get
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
      - in: query
        name: recursive
        description: Get a Tree Recursively
      - in: path
        name: repo
        description: Name of repository
      - in: path
        name: shaCode
        description: Tree SHA
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Git
      - Trees
      - Shacode
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