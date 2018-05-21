---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts_plugins_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts Plugins Conditions Policies Policy  . Format
      description: "This API endpoint allows you to create Plugins conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on creating conditions for plugins.\n\nAll
        fields are required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D
        (defaults to false).\n\nname: A title for your condition.\n\nenabled: The
        status of your condition (optional).\n\nentities: An array of instance IDs
        associated with your condition.\n\nmetric_description: A title for the metric
        to display in notifications.\n\nmetric: The metric to evaluate on.\n\nvalue_function:
        min, max, average, sample_size, total, percent\n\nrunbook_url: Runbook URL
        to display in notifications (optional).\n\nterms[duration] (in minutes): 5,
        10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
        critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
        all, any.\n\nplugin[id]: The ID of the plugin.\n\nplugin[guid]: The GUID of
        the plugin."
      operationId: postAlertsPluginsConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-plugins-conditionspoliciespolicy-idformat-post
      parameters:
      - in: body
        name: plugins_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
  /alerts_plugins_conditions/{id}.{format}:
    put:
      summary: Put Alerts Plugins Conditions  . Format
      description: "This API endpoint allows you to update Plugins conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        Alerts Plugins Conditions &gt; Create for an explanation of the field values
        ued in this command or the online document on\nupdating conditions for plugins."
      operationId: putAlertsPluginsConditions.Format
      x-api-path-slug: alerts-plugins-conditionsidformat-put
      parameters:
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      - in: body
        name: plugins_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions
      - ""
      - .
      - Format
  /alerts_plugins_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts Plugins Conditions Condition  . Format
      description: "This API endpoint allows you to delete Plugins conditions associated
        with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting Plugins conditions."
      operationId: deleteAlertsPluginsConditionsCondition.Format
      x-api-path-slug: alerts-plugins-conditionscondition-idformat-delete
      parameters:
      - in: path
        name: condition_id
        description: Alerts condition ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_plugins_conditions.{format}:
    get:
      summary: Get Alerts Plugins Conditions. Format
      description: "This API endpoint allows you to list the Plugins conditions for
        your alert policy.\n\nSee our documentation for a discussion on \noutput pagination."
      operationId: getAlertsPluginsConditions.Format
      x-api-path-slug: alerts-plugins-conditionsformat-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      - in: query
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions.
      - Format
  /alerts_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts Conditions Policies Policy  . Format
      description: "This API endpoint allows you to create conditions for your alert
        policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our documentation
        for a discussion on creating conditions for policies.\n\n\nAll fields are
        required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D (defaults
        to false), \u201Cuser_defined\u201D.\n\ntype: apm_app_metric, apm_kt_metric,
        servers_metric, browser_metric, mobile_metric.\n\nname: A title for your condition.\n\nenabled:
        The status of your condition (optional).\n\nentities: An array of instance
        IDs associated with your condition.\n\nmetric: The metric field accepts parameters
        based on the condition type selected as follows:\n\n\_\_When apm_app_metric:
        apdex, error_percentage, response_time_web, response_time_background, throughput_web,
        throughput_background, user_defined.\n\n\_\_When apm_kt_metric: apdex, error_percentage,
        error_count, response_time, throughput.\n\n\_\_When servers_metric: cpu_percentage,
        disk_io_percentage, memory_percentage, fullest_disk_percentage, load_average_one_minute,
        user_defined.\n\n\_\_When browser_metric: end_user_apdex, total_page_load,
        page_rendering, web_application, network, dom_processing, request_queuing,
        ajax_response_time, page_views_with_js_errors, page_view_throughput, ajax_throughput,
        user_defined.\n\n\_\_When mobile_metric: database, images, json, network,
        view_loading, network_error_percentage, status_error_percentage, mobile_crash_rate,
        user_defined.\n\nrunbook_url: Runbook URL to display in notifications (optional).\n\nterms[duration]
        (in minutes): 5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
        critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
        all, any.\n\nuser_defined[metric]: A custom metric to be evaluated.\n\nuser_defined[value_function]:
        average, min, max, total, sample_size."
      operationId: postAlertsConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-conditionspoliciespolicy-idformat-post
      parameters:
      - in: body
        name: condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
  /alerts_conditions/{id}.{format}:
    put:
      summary: Put Alerts Conditions  . Format
      description: "This API endpoint allows you to update conditions for your alert
        policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee Alerts Conditions
        &gt; Create for an explanation of the field values or the online \ndocumentation
        on updating conditions for policies."
      operationId: putAlertsConditions.Format
      x-api-path-slug: alerts-conditionsidformat-put
      parameters:
      - in: body
        name: condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Conditions
      - ""
      - .
      - Format
  /alerts_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts Conditions Condition  . Format
      description: "This API endpoint allows you to delete conditions associated with
        your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting conditions."
      operationId: deleteAlertsConditionsCondition.Format
      x-api-path-slug: alerts-conditionscondition-idformat-delete
      parameters:
      - in: path
        name: condition_id
        description: Alerts condition ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_conditions.{format}:
    get:
      summary: Get Alerts Conditions. Format
      description: "This API endpoint allows you to list the conditions for your alert
        policy.\n\nSee our documentation for a discussion on \noutput pagination."
      operationId: getAlertsConditions.Format
      x-api-path-slug: alerts-conditionsformat-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      - in: query
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Conditions.
      - Format
  /alerts_entity_conditions/{entity_id}.{format}:
    get:
      summary: Get Alerts Entity Conditions Entity  . Format
      description: |-
        This API endpoint allows you to list the Alerts conditions an entity is part of.

        Entity type options (Synthetics is not yet supported):

        BrowserApplication

        Application

        MobileApplication

        Server

        KeyTransaction

        Plugin
      operationId: getAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-idformat-get
      parameters:
      - in: path
        name: entity_id
        description: Entity ID
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
    put:
      summary: Put Alerts Entity Conditions Entity  . Format
      description: "This API endpoint allows you to add an entity to a specified Alerts
        condition.\n\nNote: Admin User\u2019s API Key is required.\n \n  Entity type
        options (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
      operationId: putAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-idformat-put
      parameters:
      - in: query
        name: condition_id
        description: Alerts condition ID
        type: integer
      - in: path
        name: entity_id
        description: Entity id to add
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
    delete:
      summary: Delete Alerts Entity Conditions Entity  . Format
      description: "This API endpoint allows you to disassociate an entity with a
        specified Alerts condition.\n\nNote: Admin User\u2019s API Key is required.\n\nEntity
        type options (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
      operationId: deleteAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-idformat-delete
      parameters:
      - in: query
        name: condition_id
        description: Alerts condition ID
        type: integer
      - in: path
        name: entity_id
        description: Entity id to remove
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
  /alerts_external_service_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts External Service Conditions Policies Policy  . Format
      description: "This API endpoint allows you to create external service conditions
        for your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on creating conditions for external services.\n\nAll
        fields are required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D
        (defaults to false).\n\ntype: apm_external_service, mobile_external_service.\n\nname:
        A title for your condition.\n\nenabled: The status of your condition (optional).\n\nentities:
        An array of instance IDs associated with your condition.\n\nexternal_service_url:
        The URL of the external service. Must not include protocol (\u201Cexample.com\u201D,
        not \u201Chttps://example.com\u201D)\n\nmetric: The metric field accepts parameters
        based on the condition type selected as follows:\n\n\_\_When apm_external_service:
        response_time_average, response_time_minimum, response_time_maximum, throughput.\n\n\_\_When
        mobile_external_service: response_time_average, response_time_minimum, response_time_maximum,
        throughput, network_failure_percentage, http_status_error_percentage.\n\nrunbook_url:
        Runbook URL to display in notifications (optional).\n\nterms[duration] (in
        minutes): 5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
        critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
        all, any."
      operationId: postAlertsExternalServiceConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-external-service-conditionspoliciespolicy-idformat-post
      parameters:
      - in: body
        name: external_service_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - External
      - Service
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
  /alerts_external_service_conditions/{id}.{format}:
    put:
      summary: Put Alerts External Service Conditions  . Format
      description: "This API endpoint allows you to update external service conditions
        for your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        Alerts External Service Conditions &gt; Create for an explanation of the field
        values used in this command or the online documentation on\nupdating conditions
        for external services."
      operationId: putAlertsExternalServiceConditions.Format
      x-api-path-slug: alerts-external-service-conditionsidformat-put
      parameters:
      - in: body
        name: external_service_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - External
      - Service
      - Conditions
      - ""
      - .
      - Format
  /alerts_external_service_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts External Service Conditions Condition  . Format
      description: "This API endpoint allows you to delete external service conditions
        associated with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting External services conditions."
      operationId: deleteAlertsExternalServiceConditionsCondition.Format
      x-api-path-slug: alerts-external-service-conditionscondition-idformat-delete
      parameters:
      - in: path
        name: condition_id
        description: Alerts condition ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - External
      - Service
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_external_service_conditions.{format}:
    get:
      summary: Get Alerts External Service Conditions. Format
      description: "This API endpoint allows you to list the external service conditions
        for your alert policy.\n\nSee our documentation for a discussion on \n output
        pagination."
      operationId: getAlertsExternalServiceConditions.Format
      x-api-path-slug: alerts-external-service-conditionsformat-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      - in: query
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - External
      - Service
      - Conditions.
      - Format
  /alerts_synthetics_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts Synthetics Conditions Policies Policy  . Format
      description: "This API endpoint allows you to create Synthetics conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on creating Synthetic conditions.\n\nAll
        fields are required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D
        (defaults to false).\n\nname: A title for your condition.\n\nmonitor_id: The
        GUID of the Synthetics monitor to alert on.\n\nrunbook_url: Runbook URL to
        display in notifications (optional).\n\nenabled: The status of your condition
        (optional)."
      operationId: postAlertsSyntheticsConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-synthetics-conditionspoliciespolicy-idformat-post
      parameters:
      - in: path
        name: policy_id
        description: Alerts policy ID
        type: integer
      - in: body
        name: synthetics_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Synthetics
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
  /alerts_synthetics_conditions/{id}.{format}:
    put:
      summary: Put Alerts Synthetics Conditions  . Format
      description: "This API endpoint allows you to update Synthetics conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on updating Synthetic conditions.\n\nSee
        Alerts Synthetics Conditions &gt; Create for an explanation of the field values
        used in this command."
      operationId: putAlertsSyntheticsConditions.Format
      x-api-path-slug: alerts-synthetics-conditionsidformat-put
      parameters:
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      - in: body
        name: synthetics_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Synthetics
      - Conditions
      - ""
      - .
      - Format
  /alerts_synthetics_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts Synthetics Conditions Condition  . Format
      description: "This API endpoint allows you to delete Synthetics conditions associated
        with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting Synthetic conditions."
      operationId: deleteAlertsSyntheticsConditionsCondition.Format
      x-api-path-slug: alerts-synthetics-conditionscondition-idformat-delete
      parameters:
      - in: path
        name: condition_id
        description: Alerts condition ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Synthetics
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_synthetics_conditions.{format}:
    get:
      summary: Get Alerts Synthetics Conditions. Format
      description: |-
        This API endpoint allows you to list the Synthetics conditions for your alert policy.

        See our documentation for a discussion on listing Synthetic conditions
        and  output pagination.
      operationId: getAlertsSyntheticsConditions.Format
      x-api-path-slug: alerts-synthetics-conditionsformat-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      - in: query
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Synthetics
      - Conditions.
      - Format
---