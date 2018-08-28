swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RecordLifecycleActionHeartbeat:
    get:
      summary: Record Lifecycle Action Heartbeat
      description: Records a heartbeat for the lifecycle action associated with the
        specified token or instance.
      operationId: recordLifecycleActionHeartbeat
      x-api-path-slug: actionrecordlifecycleactionheartbeat-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group for the hook
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: LifecycleActionToken
        description: A token that uniquely identifies a specific lifecycle action
          associated with an instance
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle