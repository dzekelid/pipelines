swagger: "2.0"
x-collection-name: Codefresh
x-complete: 1
info:
  title: Codefresh API
  description: codefresh-api-swagger2-0-specification
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pipelines:
    get:
      summary: Get Pipelines
      description: Get pipelines.
      operationId: getPipelines
      x-api-path-slug: pipelines-get
      responses:
        200:
          description: OK
      tags:
      - Pipelines
    post:
      summary: Post Pipelines
      description: Post pipelines.
      operationId: postPipelines
      x-api-path-slug: pipelines-post
      responses:
        200:
          description: OK
      tags:
      - Pipelines
  /pipelines/{name}:
    get:
      summary: Get Pipelines Name
      description: Get pipelines name.
      operationId: getPipelinesName
      x-api-path-slug: pipelinesname-get
      parameters:
      - in: path
        name: name
        description: Name of pipeline
      responses:
        200:
          description: OK
      tags:
      - Pipelines
      - Name
    put:
      summary: Put Pipelines Name
      description: Put pipelines name.
      operationId: putPipelinesName
      x-api-path-slug: pipelinesname-put
      parameters:
      - in: path
        name: name
        description: Name of pipeline
      responses:
        200:
          description: OK
      tags:
      - Pipelines
      - Name
    delete:
      summary: Delete Pipelines Name
      description: Delete pipelines name.
      operationId: deletePipelinesName
      x-api-path-slug: pipelinesname-delete
      parameters:
      - in: path
        name: name
        description: Name of pipeline
      responses:
        200:
          description: OK
      tags:
      - Pipelines
      - Name