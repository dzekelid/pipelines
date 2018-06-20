---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Update Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts Known Host Uu
  description: Put repositories username repo slug pipelines config ssh known hosts
    known host uu
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/pipelines/:
    get:
      summary: Get Repositories Username Repo Slug Pipelines
      description: Get repositories username repo slug pipelines
      operationId: getRepositoriesUsernameRepoSlugPipelines
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-get
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
    post:
      summary: Add Repositories Username Repo Slug Pipelines
      description: "Endpoint to create and initiate a pipeline. \nThere are a couple
        of different options to initiate a pipeline, where the payload of the request
        will determine which type of pipeline will be instantiated.\n# Trigger a Pipeline
        for a branch or tag\nOne way to trigger pipelines is by specifying the reference
        for which you want to trigger a pipeline (e.g. a branch or tag). \nThe specified
        reference will be used to determine which pipeline definition from the `bitbucket-pipelines.yml`
        file will be applied to initiate the pipeline. The pipeline will then do a
        clone of the repository and checkout the latest revision of the specified
        reference.\n\n### Example\n\n```\n$ curl -X POST -is -u username:password
        \\\n  -H 'Content-Type: application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
        \\\n  -d '\n  {\n    \"target\": {\n      \"ref_type\": \"branch\", \n      \"type\":
        \"pipeline_ref_target\", \n      \"ref_name\": \"master\"\n    }\n  }'\n```\n#
        Trigger a Pipeline for a commit on a branch or tag\nYou can initiate a pipeline
        for a specific commit and in the context of a specified reference (e.g. a
        branch, tag or bookmark).\nThe specified reference will be used to determine
        which pipeline definition from the bitbucket-pipelines.yml file will be applied
        to initiate the pipeline. The pipeline will clone the repository and then
        do a checkout the specified reference. \n\nThe following reference types are
        supported:\n\n* `branch` \n* `named_branch`\n* `bookmark` \n * `tag`\n\n###
        Example\n\n```\n$ curl -X POST -is -u username:password \\\n  -H 'Content-Type:
        application/json' \\\n  https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
        \\\n  -d '\n  {\n    \"target\": {\n      \"commit\": {\n        \"type\":
        \"commit\", \n        \"hash\": \"ce5b7431602f7cbba007062eeb55225c6e18e956\"\n
        \     }, \n      \"ref_type\": \"branch\", \n      \"type\": \"pipeline_ref_target\",
        \n      \"ref_name\": \"master\"\n    }\n  }'\n```\n# Trigger a specific pipeline
        definition for a commit\nYou can trigger a specific pipeline that is defined
        in your `bitbucket-pipelines.yml` file for a specific commit. \nIn addition
        to the commit revision, you specify the type and pattern of the selector that
        identifies the pipeline definition. The resulting pipeline will then clone
        the repository and checkout the specified revision.\n\n### Example\n\n```\n$
        curl -X POST -is -u username:password \\\n  -H 'Content-Type: application/json'
        \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
        \\\n -d '\n  {\n     \"target\": {\n      \"commit\": {\n         \"hash\":\"a3c4e02c9a3755eccdc3764e6ea13facdf30f923\",\n
        \        \"type\":\"commit\"\n       },\n        \"selector\": {\n           \"type\":\"custom\",\n
        \             \"pattern\":\"Deploy to production\"\n          },\n        \"type\":\"pipeline_commit_target\"\n
        \  }\n  }'\n```\n# Trigger a specific pipeline definition for a commit on
        a branch or tag\nYou can trigger a specific pipeline that is defined in your
        `bitbucket-pipelines.yml` file for a specific commit in the context of a specified
        reference. \nIn addition to the commit revision, you specify the type and
        pattern of the selector that identifies the pipeline definition, as well as
        the reference information. The resulting pipeline will then clone the repository
        a checkout the specified reference.\n\n### Example\n\n```\n$ curl -X POST
        -is -u username:password \\\n  -H 'Content-Type: application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
        \\\n -d '\n  {\n     \"target\": {\n      \"commit\": {\n         \"hash\":\"a3c4e02c9a3755eccdc3764e6ea13facdf30f923\",\n
        \        \"type\":\"commit\"\n       },\n       \"selector\": {\n          \"type\":
        \"custom\",\n          \"pattern\": \"Deploy to production\"\n       },\n
        \      \"type\": \"pipeline_ref_target\",\n       \"ref_name\": \"master\",\n
        \      \"ref_type\": \"branch\"\n     }\n  }'\n```"
      operationId: postRepositoriesUsernameRepoSlugPipelines
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-post
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      - in: body
        name: _body
        description: The pipeline to initiate
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
  /repositories/{username}/{repo_slug}/pipelines/{pipeline_uuid}:
    get:
      summary: Get Repositories Username Repo Slug Pipelines Pipeline Uu
      description: Get repositories username repo slug pipelines pipeline uu
      operationId: getRepositoriesUsernameRepoSlugPipelinesPipelineUu
      x-api-path-slug: repositoriesusernamerepo-slugpipelinespipeline-uuid-get
      parameters:
      - in: path
        name: pipeline_uuid
        description: The pipeline UUID
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Pipeline
      - Uu
  /repositories/{username}/{repo_slug}/pipelines/{pipeline_uuid}/steps/:
    get:
      summary: Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
      description: Get repositories username repo slug pipelines pipeline uu steps
      operationId: getRepositoriesUsernameRepoSlugPipelinesPipelineUuSteps
      x-api-path-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get
      parameters:
      - in: path
        name: pipeline_uuid
        description: The UUID of the pipeline
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Pipeline
      - Uu
      - Steps
  /repositories/{username}/{repo_slug}/pipelines/{pipeline_uuid}/steps/{step_uuid}:
    get:
      summary: Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps Step
        Uu
      description: Get repositories username repo slug pipelines pipeline uu steps
        step uu
      operationId: getRepositoriesUsernameRepoSlugPipelinesPipelineUuStepsStepUu
      x-api-path-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get
      parameters:
      - in: path
        name: pipeline_uuid
        description: The UUID of the pipeline
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: step_uuid
        description: The UUID of the step
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Pipeline
      - Uu
      - Steps
      - Step
      - Uu
  /repositories/{username}/{repo_slug}/pipelines/{pipeline_uuid}/steps/{step_uuid}/log:
    get:
      summary: Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps Step
        Uu Log
      description: |-
        Retrieve the log file for a given step of a pipeline.

        This endpoint supports (and encourages!) the use of [HTTP Range requests](https://tools.ietf.org/html/rfc7233) to deal with potentially very large log files.
      operationId: getRepositoriesUsernameRepoSlugPipelinesPipelineUuStepsStepUuLog
      x-api-path-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get
      parameters:
      - in: path
        name: pipeline_uuid
        description: The UUID of the pipeline
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: step_uuid
        description: The UUID of the step
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Pipeline
      - Uu
      - Steps
      - Step
      - Uu
      - Log
  /repositories/{username}/{repo_slug}/pipelines/{pipeline_uuid}/stopPipeline:
    post:
      summary: Add Repositories Username Repo Slug Pipelines Pipeline Uu Stoppipeline
      description: Signal the stop of a pipeline and all of its steps that not have
        completed yet.
      operationId: postRepositoriesUsernameRepoSlugPipelinesPipelineUuStoppipeline
      x-api-path-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post
      parameters:
      - in: path
        name: pipeline_uuid
        description: The UUID of the pipeline
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Pipeline
      - Uu
      - Stoppipeline
  /repositories/{username}/{repo_slug}/pipelines_config:
    get:
      summary: Get Repositories Username Repo Slug Pipelines Config
      description: Get repositories username repo slug pipelines config
      operationId: getRepositoriesUsernameRepoSlugPipelinesConfig
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-config-get
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
    put:
      summary: Update Repositories Username Repo Slug Pipelines Config
      description: Update the pipelines configuration for a repository.
      operationId: putRepositoriesUsernameRepoSlugPipelinesConfig
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-config-put
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      - in: body
        name: _body
        description: The updated repository pipelines configuration
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
  /repositories/{username}/{repo_slug}/pipelines_config/ssh/key_pair:
    delete:
      summary: Delete Repositories Username Repo Slug Pipelines Config Ssh Key Pair
      description: Delete repositories username repo slug pipelines config ssh key
        pair
      operationId: deleteRepositoriesUsernameRepoSlugPipelinesConfigSshKeyPair
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-delete
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Key
      - Pair
    get:
      summary: Get Repositories Username Repo Slug Pipelines Config Ssh Key Pair
      description: Retrieve the repository SSH key pair excluding the SSH private
        key. The private key is a write only field and will never be exposed in the
        logs or the REST API.
      operationId: getRepositoriesUsernameRepoSlugPipelinesConfigSshKeyPair
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-get
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Key
      - Pair
    put:
      summary: Update Repositories Username Repo Slug Pipelines Config Ssh Key Pair
      description: Create or update the repository SSH key pair. The private key will
        be set as a default SSH identity in your build container.
      operationId: putRepositoriesUsernameRepoSlugPipelinesConfigSshKeyPair
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-put
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      - in: body
        name: _body
        description: The created or updated SSH key pair
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Key
      - Pair
  /repositories/{username}/{repo_slug}/pipelines_config/ssh/known_hosts/:
    get:
      summary: Get Repositories Username Repo Slug Pipelines Config Ssh Known Hosts
      description: Get repositories username repo slug pipelines config ssh known
        hosts
      operationId: getRepositoriesUsernameRepoSlugPipelinesConfigSshKnownHosts
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hosts-get
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Known
      - Hosts
    post:
      summary: Add Repositories Username Repo Slug Pipelines Config Ssh Known Hosts
      description: Post repositories username repo slug pipelines config ssh known
        hosts
      operationId: postRepositoriesUsernameRepoSlugPipelinesConfigSshKnownHosts
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hosts-post
      parameters:
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      - in: body
        name: _body
        description: The known host to create
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Known
      - Hosts
  /repositories/{username}/{repo_slug}/pipelines_config/ssh/known_hosts/{known_host_uuid}:
    delete:
      summary: Delete Repositories Username Repo Slug Pipelines Config Ssh Known Hosts
        Known Host Uu
      description: Delete repositories username repo slug pipelines config ssh known
        hosts known host uu
      operationId: deleteRepositoriesUsernameRepoSlugPipelinesConfigSshKnownHostsKnownHostUu
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-delete
      parameters:
      - in: path
        name: known_host_uuid
        description: The UUID of the known host to delete
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Known
      - Hosts
      - Known
      - Host
      - Uu
    get:
      summary: Get Repositories Username Repo Slug Pipelines Config Ssh Known Hosts
        Known Host Uu
      description: Get repositories username repo slug pipelines config ssh known
        hosts known host uu
      operationId: getRepositoriesUsernameRepoSlugPipelinesConfigSshKnownHostsKnownHostUu
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-get
      parameters:
      - in: path
        name: known_host_uuid
        description: The UUID of the known host to retrieve
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Known
      - Hosts
      - Known
      - Host
      - Uu
    put:
      summary: Update Repositories Username Repo Slug Pipelines Config Ssh Known Hosts
        Known Host Uu
      description: Put repositories username repo slug pipelines config ssh known
        hosts known host uu
      operationId: putRepositoriesUsernameRepoSlugPipelinesConfigSshKnownHostsKnownHostUu
      x-api-path-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-put
      parameters:
      - in: path
        name: known_host_uuid
        description: The UUID of the known host to update
      - in: path
        name: repo_slug
        description: The repository
      - in: path
        name: username
        description: The account
      - in: body
        name: _body
        description: The updated known host
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Pipelines
      - Config
      - Ssh
      - Known
      - Hosts
      - Known
      - Host
      - Uu
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