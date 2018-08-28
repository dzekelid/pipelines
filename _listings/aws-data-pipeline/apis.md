---
name: AWS Data Pipeline
x-slug: aws-data-pipeline
description: AWS Data Pipeline is a web service that helps you reliably process and
  move data between different AWS compute and storage services, as well as on-premise
  data sources, at specified intervals. With AWS Data Pipeline, you can regularly
  access your data where it&rsquo;s stored, transform and process it at scale, and
  efficiently transfer the results to AWS services such as Amazon S3, Amazon RDS,
  Amazon DynamoDB, and Amazon EMR.AWS Data Pipeline helps you easily create complex
  data processing workloads that are fault tolerant, repeatable, and highly available.
  You don&rsquo;t have to worry about ensuring resource availability, managing inter-task
  dependencies, retrying transient failures or timeouts in individual tasks, or creating
  a failure notification system. AWS Data Pipeline also allows you to move and process
  data that was previously locked up in on-premise data silos.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Pipelines
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Data Pipeline API - Activate Pipeline
  x-api-slug: actionactivatepipeline-get
  description: Validates the specified pipeline and starts processing pipeline tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionactivatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionactivatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Create Pipeline
  x-api-slug: actioncreatepipeline-get
  description: Creates a new, empty pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actioncreatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actioncreatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Deactivate Pipeline
  x-api-slug: actiondeactivatepipeline-get
  description: Deactivates the specified running pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeactivatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeactivatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Delete Pipeline
  x-api-slug: actiondeletepipeline-get
  description: Deletes a pipeline, its pipeline definition, and its run history.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeletepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeletepipeline-get-openapi.md
- name: AWS Data Pipeline API - Describe Pipelines
  x-api-slug: actiondescribepipelines-get
  description: Retrieves metadata about one or more pipelines.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondescribepipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondescribepipelines-get-openapi.md
- name: AWS Data Pipeline API - Get Pipeline Definition
  x-api-slug: actiongetpipelinedefinition-get
  description: Gets the definition of the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiongetpipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiongetpipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - List Pipelines
  x-api-slug: actionlistpipelines-get
  description: Lists the pipeline identifiers for all active pipelines that you have
    permission to access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionlistpipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionlistpipelines-get-openapi.md
- name: AWS Data Pipeline API - Put Pipeline Definition
  x-api-slug: actionputpipelinedefinition-get
  description: Adds tasks, schedules, and preconditions to the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionputpipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionputpipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - Validate Pipeline Definition
  x-api-slug: actionvalidatepipelinedefinition-get
  description: Validates the specified pipeline definition to ensure that it is well
    formed and can be run without error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionvalidatepipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionvalidatepipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - Activate Pipeline
  x-api-slug: actionactivatepipeline-get
  description: Validates the specified pipeline and starts processing pipeline tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionactivatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionactivatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Create Pipeline
  x-api-slug: actioncreatepipeline-get
  description: Creates a new, empty pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actioncreatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actioncreatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Deactivate Pipeline
  x-api-slug: actiondeactivatepipeline-get
  description: Deactivates the specified running pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeactivatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeactivatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Delete Pipeline
  x-api-slug: actiondeletepipeline-get
  description: Deletes a pipeline, its pipeline definition, and its run history.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeletepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeletepipeline-get-openapi.md
- name: AWS Data Pipeline API - Describe Pipelines
  x-api-slug: actiondescribepipelines-get
  description: Retrieves metadata about one or more pipelines.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondescribepipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondescribepipelines-get-openapi.md
- name: AWS Data Pipeline API - Get Pipeline Definition
  x-api-slug: actiongetpipelinedefinition-get
  description: Gets the definition of the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiongetpipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiongetpipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - List Pipelines
  x-api-slug: actionlistpipelines-get
  description: Lists the pipeline identifiers for all active pipelines that you have
    permission to access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionlistpipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionlistpipelines-get-openapi.md
- name: AWS Data Pipeline API - Put Pipeline Definition
  x-api-slug: actionputpipelinedefinition-get
  description: Adds tasks, schedules, and preconditions to the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionputpipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionputpipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - Validate Pipeline Definition
  x-api-slug: actionvalidatepipelinedefinition-get
  description: Validates the specified pipeline definition to ensure that it is well
    formed and can be run without error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionvalidatepipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionvalidatepipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - Poll For Task
  x-api-slug: actionpollfortask-get
  description: Task runners call PollForTask to receive a task to perform from AWS
    Data Pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionpollfortask-get-openapi.md
- name: AWS Data Pipeline API - Set Task Status
  x-api-slug: actionsettaskstatus-get
  description: Task runners call SetTaskStatus to notify AWS Data Pipeline that a
    task is completed and provide information about the final status.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionsettaskstatus-get-openapi.md
- name: AWS Data Pipeline API - Activate Pipeline
  x-api-slug: actionactivatepipeline-get
  description: Validates the specified pipeline and starts processing pipeline tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionactivatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionactivatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Create Pipeline
  x-api-slug: actioncreatepipeline-get
  description: Creates a new, empty pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actioncreatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actioncreatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Deactivate Pipeline
  x-api-slug: actiondeactivatepipeline-get
  description: Deactivates the specified running pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeactivatepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeactivatepipeline-get-openapi.md
- name: AWS Data Pipeline API - Delete Pipeline
  x-api-slug: actiondeletepipeline-get
  description: Deletes a pipeline, its pipeline definition, and its run history.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeletepipeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondeletepipeline-get-openapi.md
- name: AWS Data Pipeline API - Describe Pipelines
  x-api-slug: actiondescribepipelines-get
  description: Retrieves metadata about one or more pipelines.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondescribepipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiondescribepipelines-get-openapi.md
- name: AWS Data Pipeline API - Get Pipeline Definition
  x-api-slug: actiongetpipelinedefinition-get
  description: Gets the definition of the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiongetpipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actiongetpipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - List Pipelines
  x-api-slug: actionlistpipelines-get
  description: Lists the pipeline identifiers for all active pipelines that you have
    permission to access.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionlistpipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionlistpipelines-get-openapi.md
- name: AWS Data Pipeline API - Put Pipeline Definition
  x-api-slug: actionputpipelinedefinition-get
  description: Adds tasks, schedules, and preconditions to the specified pipeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionputpipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionputpipelinedefinition-get-openapi.md
- name: AWS Data Pipeline API - Validate Pipeline Definition
  x-api-slug: actionvalidatepipelinedefinition-get
  description: Validates the specified pipeline definition to ensure that it is well
    formed and can be run without error.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Analytics_AWSDataPipeline.png
  humanURL: https://aws.amazon.com/datapipeline/
  baseURL: :///
  tags: Amazon Web Services, Stack Network, Data, API Service Provider, API Service
    Provider, API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionvalidatepipelinedefinition-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/pipelines/master/_listings/aws-data-pipeline/actionvalidatepipelinedefinition-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.config.api.gallery.streamdata.io
- type: x-api-stack
  url: http://aws.data.pipeline.stack.network
- type: x-blog
  url: http://blogs.aws.amazon.com/bigdata
- type: x-change-log
  url: http://aws.amazon.com/releasenotes/AWS-Data-Pipeline/
- type: x-documentation
  url: http://docs.aws.amazon.com/datapipeline/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/datapipeline/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=151
- type: x-pricing
  url: https://aws.amazon.com/datapipeline/pricing/
- type: x-tools
  url: http://aws.amazon.com/developertools/AWS-Data-Pipeline/
- type: x-website
  url: https://aws.amazon.com/datapipeline/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---