---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Post Projects Pipeline
  version: 1.0.0
  description: This feature was introduced in GitLab 8.14
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/pipelines:
    get:
      summary: Get Projects Pipelines
      description: This feature was introduced in GitLab 8.11.
      operationId: getV3ProjectsIdPipelines
      x-api-path-slug: v3projectsidpipelines-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      - in: query
        name: scope
        description: Either running, branches, or tags
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
  /v3/projects/{id}/pipelines/{pipeline_id}:
    get:
      summary: Get Projects Pipelines Pipeline
      description: This feature was introduced in GitLab 8.11
      operationId: getV3ProjectsIdPipelinesPipelineId
      x-api-path-slug: v3projectsidpipelinespipeline-id-get
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: pipeline_id
        description: The pipeline ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
      - Pipeline
  /v3/projects/{id}/pipelines/{pipeline_id}/retry:
    post:
      summary: Post Projects Pipelines Pipeline Retry
      description: This feature was introduced in GitLab 8.11.
      operationId: postV3ProjectsIdPipelinesPipelineIdRetry
      x-api-path-slug: v3projectsidpipelinespipeline-idretry-post
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: pipeline_id
        description: The pipeline ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
      - Pipeline
      - Retry
  /v3/projects/{id}/pipelines/{pipeline_id}/cancel:
    post:
      summary: Post Projects Pipelines Pipeline Cancel
      description: This feature was introduced in GitLab 8.11.
      operationId: postV3ProjectsIdPipelinesPipelineIdCancel
      x-api-path-slug: v3projectsidpipelinespipeline-idcancel-post
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: path
        name: pipeline_id
        description: The pipeline ID
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipelines
      - Pipeline
      - Cancel
  /v3/projects/{id}/services/pipelines-email:
    put:
      summary: Put Projects Services Pipelines Email
      description: Set pipelines-email service for project
      operationId: putV3ProjectsIdServicesPipelinesEmail
      x-api-path-slug: v3projectsidservicespipelinesemail-put
      parameters:
      - in: path
        name: id
      - in: formData
        name: notify_only_broken_builds
        description: Notify only broken builds
      - in: formData
        name: pipeline_events
      - in: formData
        name: recipients
        description: Comma-separated list of recipient email addresses
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Pipelines
      - Email
  /v3/projects/{id}/pipeline:
    post:
      summary: Post Projects Pipeline
      description: This feature was introduced in GitLab 8.14
      operationId: postV3ProjectsIdPipeline
      x-api-path-slug: v3projectsidpipeline-post
      parameters:
      - in: path
        name: id
        description: The project ID
      - in: formData
        name: ref
        description: Reference
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Pipeline
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