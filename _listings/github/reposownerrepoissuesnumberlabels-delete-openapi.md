---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Delete Repos Owner Repo Issues Number Labels
  description: Remove all labels from an issue.
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
  /repos/{owner}/{repo}/issues/{number}:
    get:
      summary: Get Repos Owner Repo Issues Number
      description: Get a single issue
      operationId: get-a-single-issue
      x-api-path-slug: reposownerrepoissuesnumber-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of issue
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
      - Issues
      - Number
    patch:
      summary: Patch Repos Owner Repo Issues Number
      description: |-
        Edit an issue.
        Issue owners and users with push access can edit an issue.
      operationId: edit-an-issueissue-owners-and-users-with-push-access-can-edit-an-issue
      x-api-path-slug: reposownerrepoissuesnumber-patch
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
        name: number
        description: Number of issue
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
      - Issues
      - Number
  /repos/{owner}/{repo}/issues/{number}/comments:
    get:
      summary: Get Repos Owner Repo Issues Number Comments
      description: List comments on an issue.
      operationId: list-comments-on-an-issue
      x-api-path-slug: reposownerrepoissuesnumbercomments-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of issue
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
      - Issues
      - Number
      - Comments
    post:
      summary: Add Repos Owner Repo Issues Number Comments
      description: Create a comment.
      operationId: create-a-comment
      x-api-path-slug: reposownerrepoissuesnumbercomments-post
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
        name: number
        description: Number of issue
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
      - Issues
      - Number
      - Comments
  /repos/{owner}/{repo}/issues/{number}/events:
    get:
      summary: Get Repos Owner Repo Issues Number Events
      description: List events for an issue.
      operationId: list-events-for-an-issue
      x-api-path-slug: reposownerrepoissuesnumberevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of issue
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
      - Issues
      - Number
      - Events
  /repos/{owner}/{repo}/issues/{number}/labels:
    delete:
      summary: Delete Repos Owner Repo Issues Number Labels
      description: Remove all labels from an issue.
      operationId: remove-all-labels-from-an-issue
      x-api-path-slug: reposownerrepoissuesnumberlabels-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of issue
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
      - Issues
      - Number
      - Labels
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