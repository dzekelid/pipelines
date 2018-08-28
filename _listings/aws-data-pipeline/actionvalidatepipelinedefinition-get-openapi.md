---
swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 0
info:
  title: AWS Data Pipeline API Validate Pipeline Definition
  version: 1.0.0
  description: Validates the specified pipeline definition to ensure that it is well
    formed and can be run without error.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ActivatePipeline:
    get:
      summary: Activate Pipeline
      description: Validates the specified pipeline and starts processing pipeline
        tasks.
      operationId: activatePipeline
      x-api-path-slug: actionactivatepipeline-get
      parameters:
      - in: query
        name: parameterValues
        description: A list of parameter values to pass to the pipeline at activation
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: startTimestamp
        description: The date and time to resume the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=CreatePipeline:
    get:
      summary: Create Pipeline
      description: Creates a new, empty pipeline.
      operationId: createPipeline
      x-api-path-slug: actioncreatepipeline-get
      parameters:
      - in: query
        name: description
        description: The description for the pipeline
        type: string
      - in: query
        name: name
        description: The name for the pipeline
        type: string
      - in: query
        name: tags
        description: A list of tags to associate with the pipeline at creation
        type: string
      - in: query
        name: uniqueId
        description: A unique identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DeactivatePipeline:
    get:
      summary: Deactivate Pipeline
      description: Deactivates the specified running pipeline.
      operationId: deactivatePipeline
      x-api-path-slug: actiondeactivatepipeline-get
      parameters:
      - in: query
        name: cancelActive
        description: Indicates whether to cancel any running objects
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DeletePipeline:
    get:
      summary: Delete Pipeline
      description: Deletes a pipeline, its pipeline definition, and its run history.
      operationId: deletePipeline
      x-api-path-slug: actiondeletepipeline-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DescribePipelines:
    get:
      summary: Describe Pipelines
      description: Retrieves metadata about one or more pipelines.
      operationId: describePipelines
      x-api-path-slug: actiondescribepipelines-get
      parameters:
      - in: query
        name: pipelineIds
        description: The IDs of the pipelines to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=GetPipelineDefinition:
    get:
      summary: Get Pipeline Definition
      description: Gets the definition of the specified pipeline.
      operationId: getPipelineDefinition
      x-api-path-slug: actiongetpipelinedefinition-get
      parameters:
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: version
        description: The version of the pipeline definition to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=ListPipelines:
    get:
      summary: List Pipelines
      description: Lists the pipeline identifiers for all active pipelines that you
        have permission to access.
      operationId: listPipelines
      x-api-path-slug: actionlistpipelines-get
      parameters:
      - in: query
        name: marker
        description: The starting point for the results to be returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=PutPipelineDefinition:
    get:
      summary: Put Pipeline Definition
      description: Adds tasks, schedules, and preconditions to the specified pipeline.
      operationId: putPipelineDefinition
      x-api-path-slug: actionputpipelinedefinition-get
      parameters:
      - in: query
        name: parameterObjects
        description: The parameter objects used with the pipeline
        type: string
      - in: query
        name: parameterValues
        description: The parameter values used with the pipeline
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: pipelineObjects
        description: The objects that define the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=ValidatePipelineDefinition:
    get:
      summary: Validate Pipeline Definition
      description: Validates the specified pipeline definition to ensure that it is
        well formed and can be run without error.
      operationId: validatePipelineDefinition
      x-api-path-slug: actionvalidatepipelinedefinition-get
      parameters:
      - in: query
        name: parameterObjects
        description: The parameter objects used with the pipeline
        type: string
      - in: query
        name: parameterValues
        description: The parameter values used with the pipeline
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline
        type: string
      - in: query
        name: pipelineObjects
        description: The objects that define the pipeline changes to validate against
          the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=PollForTask:
    get:
      summary: Poll For Task
      description: Task runners call PollForTask to receive a task to perform from
        AWS Data Pipeline.
      operationId: pollForTask
      x-api-path-slug: actionpollfortask-get
      parameters:
      - in: query
        name: hostname
        description: The public DNS name of the calling task runner
        type: string
      - in: query
        name: instanceIdentity
        description: Identity information for the EC2 instance that is hosting the
          task runner
        type: string
      - in: query
        name: workerGroup
        description: The type of task the task runner is configured to accept and
          process
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
  /?Action=SetTaskStatus:
    get:
      summary: Set Task Status
      description: Task runners call SetTaskStatus to notify AWS Data Pipeline that
        a task is completed and provide information about the final status.
      operationId: setTaskStatus
      x-api-path-slug: actionsettaskstatus-get
      parameters:
      - in: query
        name: errorId
        description: If an error occurred during the task, this value specifies the
          error code
        type: string
      - in: query
        name: errorMessage
        description: If an error occurred during the task, this value specifies a
          text description of the error
        type: string
      - in: query
        name: errorStackTrace
        description: If an error occurred during the task, this value specifies the
          stack trace associated with the error
        type: string
      - in: query
        name: taskId
        description: The ID of the task assigned to the task runner
        type: string
      - in: query
        name: taskStatus
        description: If FINISHED, the task successfully completed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks
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