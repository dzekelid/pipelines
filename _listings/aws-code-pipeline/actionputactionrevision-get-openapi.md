---
swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 0
info:
  title: AWS Code Pipeline API Put Action Revision
  version: 1.0.0
  description: Provides information to AWS CodePipeline about new revisions to a source.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListPipelines:
    get:
      summary: List Pipelines
      description: Gets a summary of all of the pipelines associated with your account.
      operationId: listPipelines
      x-api-path-slug: actionlistpipelines-get
      parameters:
      - in: query
        name: AllocationId.N
        description: '[EC2-VPC] One or more allocation IDs'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous list pipelines
          call, which can be            used to return the next set of pipelines in
          the list
        type: string
      - in: query
        name: PublicIp.N
        description: '[EC2-Classic] One or more Elastic IP addresses'
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Pipelines
  /?Action=CreatePipeline:
    get:
      summary: Create Pipeline
      description: Creates a pipeline.
      operationId: createPipeline
      x-api-path-slug: actioncreatepipeline-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of snapshot results returned by DescribeSnapshots
          in      paginated output
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeSnapshots
          request where MaxResults was used and the      results exceeded the value
          of that parameter
        type: string
      - in: query
        name: Owner.N
        description: Returns the snapshots owned by the specified owner
        type: string
      - in: query
        name: pipeline
        description: Represents the structure of actions and stages to be performed
          in the            pipeline
        type: string
      - in: query
        name: RestorableBy.N
        description: One or more AWS accounts IDs that can create volumes from the
          snapshot
        type: string
      - in: query
        name: SnapshotId.N
        description: One or more snapshot IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=DeletePipeline:
    get:
      summary: Delete Pipeline
      description: Deletes the specified pipeline.
      operationId: deletePipeline
      x-api-path-slug: actiondeletepipeline-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of volume results returned by DescribeVolumes
          in paginated      output
        type: string
      - in: query
        name: name
        description: The name of the pipeline to be deleted
        type: string
      - in: query
        name: NextToken
        description: The NextToken value returned from a previous paginated        DescribeVolumes
          request where MaxResults was used and the results      exceeded the value
          of that parameter
        type: string
      - in: query
        name: VolumeId.N
        description: One or more volume IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=GetPipeline:
    get:
      summary: Get Pipeline
      description: Returns the metadata, structure, stages, and actions of a pipeline.
      operationId: getPipeline
      x-api-path-slug: actiongetpipeline-get
      parameters:
      - in: query
        name: Attribute
        description: The snapshot attribute to modify
        type: string
      - in: query
        name: CreateVolumePermission
        description: A JSON representation of the snapshot attribute modification
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline for which you want to get information
        type: string
      - in: query
        name: OperationType
        description: The type of operation to perform to the attribute
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      - in: query
        name: UserGroup.N
        description: The group to modify for the snapshot
        type: string
      - in: query
        name: UserId.N
        description: The account ID to modify for the snapshot
        type: string
      - in: query
        name: version
        description: The version number of the pipeline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=GetPipelineExecution:
    get:
      summary: Get Pipeline Execution
      description: |-
        Returns information about an execution of a pipeline, including details about
                    artifacts, the pipeline execution ID, and the name, version, and status of the
                    pipeline.
      operationId: getPipelineExecution
      x-api-path-slug: actiongetpipelineexecution-get
      parameters:
      - in: query
        name: AutoEnableIO
        description: Indicates whether the volume should be auto-enabled for I/O operations
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: pipelineExecutionId
        description: The ID of the pipeline execution about which you want to get
          execution            details
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline about which you want to get execution
          details
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
      - Execution
  /?Action=GetPipelineState:
    get:
      summary: Get Pipeline State
      description: |-
        Returns information about the state of a pipeline, including the stages and
                    actions.
      operationId: getPipelineState
      x-api-path-slug: actiongetpipelinestate-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline about which you want to get information
        type: string
      - in: query
        name: SnapshotId
        description: The ID of the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
      - State
  /?Action=StartPipelineExecution:
    get:
      summary: Start Pipeline Execution
      description: Starts the specified pipeline.
      operationId: startPipelineExecution
      x-api-path-slug: actionstartpipelineexecution-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: name
        description: The name of the pipeline to start
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Start
      - Pipeline
      - Execution
  /?Action=UpdatePipeline:
    get:
      summary: Update Pipeline
      description: Updates a specified pipeline with edits or changes to its structure.
      operationId: updatePipeline
      x-api-path-slug: actionupdatepipeline-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute of the network interface
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: pipeline
        description: The name of the pipeline to be updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Pipeline
  /?Action=ListActionTypes:
    get:
      summary: List Action Types
      description: |-
        Gets a summary of all AWS CodePipeline action types associated with your
                    account.
      operationId: listActionTypes
      x-api-path-slug: actionlistactiontypes-get
      parameters:
      - in: query
        name: actionOwnerFilter
        description: Filters the list of action types to those created by a specified
          entity
        type: string
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: AllowReassociation
        description: '[EC2-VPC] For a VPC in an EC2-Classic account, specify true
          to allow an Elastic IP address that is already associated with an instance
          or network interface to be reassociated with the specified instance or network
          interface'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: NetworkInterfaceId
        description: '[EC2-VPC] The ID of the network interface'
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous list action
          types call, which can            be used to return the next set of action
          types in the list
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary or secondary private IP address to associate
          with the Elastic IP address'
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Action
      - Types
  /?Action=PollForJobs:
    get:
      summary: Poll For Jobs
      description: Returns information about any jobs for AWS CodePipeline to act
        upon.
      operationId: pollForJobs
      x-api-path-slug: actionpollforjobs-get
      parameters:
      - in: query
        name: actionTypeId
        description: Represents information about an action type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: maxBatchSize
        description: The maximum number of jobs to return in a poll for jobs call
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to use to retrieve the next page of results
        type: string
      - in: query
        name: PublicIp.N
        description: One or more Elastic IP addresses
        type: string
      - in: query
        name: queryParam
        description: A map of property names and values
        type: string
      responses:
        200:
          description: OK
      tags:
      - PollJobs
  /?Action=PutActionRevision:
    get:
      summary: Put Action Revision
      description: Provides information to AWS CodePipeline about new revisions to
        a source.
      operationId: putActionRevision
      x-api-path-slug: actionputactionrevision-get
      parameters:
      - in: query
        name: actionName
        description: The name of the action that will process the revision
        type: string
      - in: query
        name: actionRevision
        description: Represents information about the version (or revision) of an
          action
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: pipelineName
        description: The name of the pipeline that will start processing the revision
          to the            source
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      - in: query
        name: stageName
        description: The name of the stage that contains the action that will act
          upon the            revision
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Action
      - Revision
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