---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Pipelines
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines
  x-api-slug: repositoriesusernamerepo-slugpipelines-get
  description: Get repositories username repo slug pipelines
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines
  x-api-slug: repositoriesusernamerepo-slugpipelines-post
  description: "Endpoint to create and initiate a pipeline. \nThere are a couple of
    different options to initiate a pipeline, where the payload of the request will
    determine which type of pipeline will be instantiated.\n# Trigger a Pipeline for
    a branch or tag\nOne way to trigger pipelines is by specifying the reference for
    which you want to trigger a pipeline (e.g. a branch or tag). \nThe specified reference
    will be used to determine which pipeline definition from the `bitbucket-pipelines.yml`
    file will be applied to initiate the pipeline. The pipeline will then do a clone
    of the repository and checkout the latest revision of the specified reference.\n\n###
    Example\n\n```\n$ curl -X POST -is -u username:password \\\n  -H 'Content-Type:
    application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n  -d '\n  {\n    \"target\": {\n      \"ref_type\": \"branch\", \n      \"type\":
    \"pipeline_ref_target\", \n      \"ref_name\": \"master\"\n    }\n  }'\n```\n#
    Trigger a Pipeline for a commit on a branch or tag\nYou can initiate a pipeline
    for a specific commit and in the context of a specified reference (e.g. a branch,
    tag or bookmark).\nThe specified reference will be used to determine which pipeline
    definition from the bitbucket-pipelines.yml file will be applied to initiate the
    pipeline. The pipeline will clone the repository and then do a checkout the specified
    reference. \n\nThe following reference types are supported:\n\n* `branch` \n*
    `named_branch`\n* `bookmark` \n * `tag`\n\n### Example\n\n```\n$ curl -X POST
    -is -u username:password \\\n  -H 'Content-Type: application/json' \\\n  https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n  -d '\n  {\n    \"target\": {\n      \"commit\": {\n        \"type\": \"commit\",
    \n        \"hash\": \"ce5b7431602f7cbba007062eeb55225c6e18e956\"\n      }, \n
    \     \"ref_type\": \"branch\", \n      \"type\": \"pipeline_ref_target\", \n
    \     \"ref_name\": \"master\"\n    }\n  }'\n```\n# Trigger a specific pipeline
    definition for a commit\nYou can trigger a specific pipeline that is defined in
    your `bitbucket-pipelines.yml` file for a specific commit. \nIn addition to the
    commit revision, you specify the type and pattern of the selector that identifies
    the pipeline definition. The resulting pipeline will then clone the repository
    and checkout the specified revision.\n\n### Example\n\n```\n$ curl -X POST -is
    -u username:password \\\n  -H 'Content-Type: application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n -d '\n  {\n     \"target\": {\n      \"commit\": {\n         \"hash\":\"a3c4e02c9a3755eccdc3764e6ea13facdf30f923\",\n
    \        \"type\":\"commit\"\n       },\n        \"selector\": {\n           \"type\":\"custom\",\n
    \             \"pattern\":\"Deploy to production\"\n          },\n        \"type\":\"pipeline_commit_target\"\n
    \  }\n  }'\n```\n# Trigger a specific pipeline definition for a commit on a branch
    or tag\nYou can trigger a specific pipeline that is defined in your `bitbucket-pipelines.yml`
    file for a specific commit in the context of a specified reference. \nIn addition
    to the commit revision, you specify the type and pattern of the selector that
    identifies the pipeline definition, as well as the reference information. The
    resulting pipeline will then clone the repository a checkout the specified reference.\n\n###
    Example\n\n```\n$ curl -X POST -is -u username:password \\\n  -H 'Content-Type:
    application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n -d '\n  {\n     \"target\": {\n      \"commit\": {\n         \"hash\":\"a3c4e02c9a3755eccdc3764e6ea13facdf30f923\",\n
    \        \"type\":\"commit\"\n       },\n       \"selector\": {\n          \"type\":
    \"custom\",\n          \"pattern\": \"Deploy to production\"\n       },\n       \"type\":
    \"pipeline_ref_target\",\n       \"ref_name\": \"master\",\n       \"ref_type\":
    \"branch\"\n     }\n  }'\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get
  description: Get repositories username repo slug pipelines pipeline uu steps
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu steps step
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu Log
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get
  description: |-
    Retrieve the log file for a given step of a pipeline.

    This endpoint supports (and encourages!) the use of [HTTP Range requests](https://tools.ietf.org/html/rfc7233) to deal with potentially very large log files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Pipeline Uu Stoppipeline
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post
  description: Signal the stop of a pipeline and all of its steps that not have completed
    yet.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config
  x-api-slug: repositoriesusernamerepo-slugpipelines-config-get
  description: Get repositories username repo slug pipelines config
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-config-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-config-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config
  x-api-slug: repositoriesusernamerepo-slugpipelines-config-put
  description: Update the pipelines configuration for a repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-config-put-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Pipelines Config Ssh Key
    Pair
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-delete
  description: Delete repositories username repo slug pipelines config ssh key pair
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Ssh Key Pair
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-get
  description: Retrieve the repository SSH key pair excluding the SSH private key.
    The private key is a write only field and will never be exposed in the logs or
    the REST API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config Ssh Key
    Pair
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-put
  description: Create or update the repository SSH key pair. The private key will
    be set as a default SSH identity in your build container.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hosts-get
  description: Get repositories username repo slug pipelines config ssh known hosts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hosts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hosts-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hosts-post
  description: Post repositories username repo slug pipelines config ssh known hosts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hosts-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts Known Host Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-delete
  description: Delete repositories username repo slug pipelines config ssh known hosts
    known host uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts Known Host Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-get
  description: Get repositories username repo slug pipelines config ssh known hosts
    known host uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts Known Host Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-put
  description: Put repositories username repo slug pipelines config ssh known hosts
    known host uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Variables
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariables-get
  description: Get repositories username repo slug pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariables-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Config Variables
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariables-post
  description: Post repositories username repo slug pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariables-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Pipelines Config Variables
    Variable Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-delete
  description: Delete repositories username repo slug pipelines config variables variable
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Variables
    Variable Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-get
  description: Get repositories username repo slug pipelines config variables variable
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config Variables
    Variable Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-put
  description: Put repositories username repo slug pipelines config variables variable
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-put-openapi.md
- name: Bitbucket - Get Teams Username Pipelines Config Variables
  x-api-slug: teamsusernamepipelines-configvariables-get
  description: Get teams username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariables-get-openapi.md
- name: Bitbucket - Add Teams Username Pipelines Config Variables
  x-api-slug: teamsusernamepipelines-configvariables-post
  description: Post teams username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariables-post-openapi.md
- name: Bitbucket - Delete Teams Username Pipelines Config Variables Variable Uu
  x-api-slug: teamsusernamepipelines-configvariablesvariable-uuid-delete
  description: Delete teams username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-delete-openapi.md
- name: Bitbucket - Get Teams Username Pipelines Config Variables Variable Uu
  x-api-slug: teamsusernamepipelines-configvariablesvariable-uuid-get
  description: Get teams username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-get-openapi.md
- name: Bitbucket - Update Teams Username Pipelines Config Variables Variable Uu
  x-api-slug: teamsusernamepipelines-configvariablesvariable-uuid-put
  description: Put teams username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/teamsusernamepipelines-configvariablesvariable-uuid-put-openapi.md
- name: Bitbucket - Get Users Username Pipelines Config Variables
  x-api-slug: usersusernamepipelines-configvariables-get
  description: Get users username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariables-get-openapi.md
- name: Bitbucket - Add Users Username Pipelines Config Variables
  x-api-slug: usersusernamepipelines-configvariables-post
  description: Post users username pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariables-post-openapi.md
- name: Bitbucket - Delete Users Username Pipelines Config Variables Variable Uu
  x-api-slug: usersusernamepipelines-configvariablesvariable-uuid-delete
  description: Delete users username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-delete-openapi.md
- name: Bitbucket - Get Users Username Pipelines Config Variables Variable Uu
  x-api-slug: usersusernamepipelines-configvariablesvariable-uuid-get
  description: Get users username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-get-openapi.md
- name: Bitbucket - Update Users Username Pipelines Config Variables Variable Uu
  x-api-slug: usersusernamepipelines-configvariablesvariable-uuid-put
  description: Put users username pipelines config variables variable uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/usersusernamepipelines-configvariablesvariable-uuid-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get
  description: Get repositories username repo slug pipelines pipeline uu steps
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu steps step
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu Log
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get
  description: |-
    Retrieve the log file for a given step of a pipeline.

    This endpoint supports (and encourages!) the use of [HTTP Range requests](https://tools.ietf.org/html/rfc7233) to deal with potentially very large log files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Pipeline Uu Stoppipeline
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post
  description: Signal the stop of a pipeline and all of its steps that not have completed
    yet.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get
  description: Get repositories username repo slug pipelines pipeline uu steps
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu steps step
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu Log
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get
  description: |-
    Retrieve the log file for a given step of a pipeline.

    This endpoint supports (and encourages!) the use of [HTTP Range requests](https://tools.ietf.org/html/rfc7233) to deal with potentially very large log files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Pipeline Uu Stoppipeline
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post
  description: Signal the stop of a pipeline and all of its steps that not have completed
    yet.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Pipeline Uu Stoppipeline
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post
  description: Signal the stop of a pipeline and all of its steps that not have completed
    yet.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu Log
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get
  description: |-
    Retrieve the log file for a given step of a pipeline.

    This endpoint supports (and encourages!) the use of [HTTP Range requests](https://tools.ietf.org/html/rfc7233) to deal with potentially very large log files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu steps step
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get
  description: Get repositories username repo slug pipelines pipeline uu steps
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---