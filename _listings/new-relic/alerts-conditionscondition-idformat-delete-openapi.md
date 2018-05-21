---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Delete Alerts Conditions Condition  . Format
  version: 1.0.0
  description: "This API endpoint allows you to delete conditions associated with
    your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our
    documentation for a discussion on deleting conditions."
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