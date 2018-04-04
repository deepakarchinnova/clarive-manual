## Forms {#forms}

### Product Backlog {#product-backlog}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |  |  |  |  |  |
| Title | title | head | 9 | X |  |  |
| Status | status | Body | 3 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| System | system | Details | 4 | X |  |  |
| Owner | owner | Details | 4 | (X) |  |  |
| --- Releated Topics |  |  |  |  |  |  |
| User Stories | product_backlog_user_stories | Header | 12 |  |  |  |
| Defects | product_backlog_defects |  |  |  |  |  |
| History | History | Details | 12 | X |  |  |
| Owner Name | Ownername | Header | 4 |  | X | X |

### Sprint {#sprint}

| Field |  | Section | Width | Mandatory | HWM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |   |  |  |  |  |
| Title | title | head | 8 | X |  |  |
| Status | status | Body | 4 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| Owner | owner | Details | 3 | (X) |  |  |
| ~~System~~ | ~~system~~ | ~~Details~~ | ~~3~~ | ~~X~~ |  |  |
| Scheduled Start Date | start_date | Body | 4 | X |  |  |
| Scheduled End Date | end_date | Body | 4 | X |  |  |
| --- Ranking Details |  |  |  |  |  |  |
| Total Story Points | total_story_points | Body | 4 |  |  |  |
| Used Story Points | used_story_points | Body | 4 |  |  |  |
| Available Story Points | available_story_points | Body | 4 |  |  |  |
| --- Timing Details |  |   |  |  |  |  |
| ~~Due Date~~ | ~~due_date~~ | ~~Body~~ | ~~3~~ |  |  |  |
| Date Opened | open_date | Body | 3 | (X) |  |  |
| Pickup Date | pickup_date | Body | 3 |  |  |  |
| Resolution Date | resolution_date | Body | 3 |  |  |  |
| Date Closed | close_date | Body | 3 |  |  |  |
| --- Releated Topics |  |   |  |  |  |  |
| User Stories | sprint_user_stories | Header | 12 |  |  |  |
| Defects | sprint_defects | Header | 12 |  |  |  |
| ~~Changesets~~ | ~~sprint_changeset~~ | ~~Header~~ | ~~6~~ |  |  |  |
| History | history | Details | 12 | X |  |  |
| Owner Name | ownername | Header | 4 |  | X | X |

### User Story {#user-story}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |  |  |  |  |  |
| Title | title | head | 9 | X |  |  |
| Status | status | Body | 3 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| Requestor | initiator | Details | 4 | X |  |  |
| Owner | owner | Details | 3 | (X) |  |  |
| Activity Type | activity_type | Body | 6 | X |  |  |
| Approved By | approver | Details | 3 |  |  | X |
| Approved On | approved_on | Body | 3 |  |  | X |
| System | system | Details | 6 | X |  |  |
| ~~Nature~~ | ~~nature~~ | ~~Details~~ | ~~6~~ | ~~X~~ |  |  |
| Product Backlog | product_backlog | Header | 6 |  |  |  |
| Sprint | sprint | Header | 3 |  |  |  |
| Changeset | changeset | Header | 3 |  | X |  |
| --- Ranking Details |  |  |  |  |  |  |
| Story Points | story_points | Body | 4 |  |  |  |
| Risk | risk | Body | 4 |  | X |  |
| Estimated Effort | estimated_effort | Body | 4 |  |  |  |
| Priority | backlog_priority | Body | 4 |  |  |  |
| Reason | reason | Body | 4 |  | X |  |
| --- Value Assessment |  |  |  |  |  |  |
| Strategic Value | strategic_value | Body | 4 |  | X |  |
| Customer Value | customer_value | Body | 4 |  | X |  |
| Competitive Value | competitive_value | Body | 4 |  | X |  |
| --- Timing Details |  |  |  |  |  |  |
| Due Date | due_date | Body | 2 |  |  |  |
| Date Opened | open_date | Body | 2 | (X) |  |  |
| Pickup Date | pickup_date | Body | 2 |  |  |  |
| Resolution Date | resolution_date | Body | 2 |  |  |  |
| Date Closed | close_date | Body | 2 |  |  |  |
| --- More Info |  |  |  |  |  |  |
| Revisions | revisions | Details | 6 |  |  |  |
| Documents | ficheros_adjuntos | Details | 6 |  |  |  |
| Files | ficherons | Details | 6 |  |  |  |
| SQL-Files | sql_files | Details | 6 |  |  |  |
| --- Releated Topics |  |  |  |  |  |  |
| Tasks | user_story_tasks | Header | 12 |  |  |  |
| History | history | Details | 12 | X |  |  |
| Owner Name | Ownername | Header | 4 |  | X | X |

* Activity Type : Requirement, Design, Development (default), Document, Testing, Other

### Defect {#defect}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |  |  |  |  |  |
| Title | title | head | 9 | X |  |  |
| Status | status | Body | 3 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| Requestor | initiator | Details | 4 | X |  |  |
| Owner | owner | Details | 3 | (X) |  |  |
| Activity Type | activity_type | Body | 6 | X |  |  |
| ~~Approved By~~ | ~~approver~~ | ~~Details~~ | ~~3~~ |  |  | ~~X~~ |
| ~~Approved On~~ | ~~approved_on~~ | ~~Body~~ | ~~3~~ |  |  | ~~X~~ |
| System | system | Details | 6 | X |  |  |
| ~~Nature~~ | ~~nature~~ | ~~Details~~ | ~~6~~ | ~~X~~ |  |  |
| Product Backlog | product_backlog | Header | 6 |  |  |  |
| Sprint | sprint | Header | 3 |  |  |  |
| Changeset | changeset | Header | 3 |  | X |  |
| --- Ranking Details |  |  |  |  |  |  |
| Story Points | story_points | Body | 4 |  |  |  |
| Risk | risk | Body | 4 |  | X |  |
| Estimated Effort | estimated_effort | Body | 4 |  |  |  |
| Priority | backlog_priority | Body | 4 |  |  |  |
| Reason | reason | Body | 4 |  | X |  |
| --- Value Assessment |  |  |  |  |  |  |
| Strategic Value | strategic_value | Body | 4 |  | X |  |
| Customer Value | customer_value | Body | 4 |  | X |  |
| Competitive Value | competitive_value | Body | 4 |  | X |  |
| --- Timing Details |  |  |  |  |  |  |
| Due Date | due_date | Body | 2 |  |  |  |
| Date Opened | open_date | Body | 2 | (X) |  |  |
| Pickup Date | pickup_date | Body | 2 |  |  |  |
| Resolution Date | resolution_date | Body | 2 |  |  |  |
| Date Closed | close_date | Body | 2 |  |  |  |
| --- More Info |  |  |  |  |  |  |
| Revisions | revisions | Details | 6 |  |  |  |
| Documents | ficheros_adjuntos | Details | 6 |  |  |  |
| Files | ficherons | Details | 6 |  |  |  |
| SQL-Files | sql_files | Details | 6 |  |  |  |
| --- Releated Topics |  |  |  |  |  |  |
| Tasks | defect_tasks | Header | 12 |  |  |  |
| History | history | Details | 12 | X |  |  |
| Owner Name | Ownername | Header | 4 |  | X | X |

### Task {#task}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |   |  |  |   |   |
| Title | title | head | 9 | X |   |   |
| Status | status | Body | 3 | X |   |   |
| Description | description | Header | 12 | X |   |   |
| User Story | user_story | Header | 12 |  |   |   |
| Defect | defect | Header | 12 |  |  |  |
| Hotfix | hotfix | Header | 12 |  |  |  |
| Owner | owner | Details | 4 | (X) |   |   |
| System | system | Details | 3 | X |  |  |
| Estimated Effort | estimated_effort | Body | 3 | X |   |   |
| Activity Type* | activity_type | Body | 6 |  |  |  |
| Vaildated By | validate_by | Details | 3 |  |  | X |
| Validated On | validated_on | Details | 3 |  |  | X |
| ~~Priority~~ | ~~priority~~ | ~~Body~~ | ~~4~~ | ~~X~~ | ~~ ~~ | ~~ ~~ |
| --- Timing Details |  |   |  |  |   |   |
| Due Date | due_date | Body | 2 |  |   |   |
| Date Opened | open_date | Body | 2 | (X) |   |   |
| Pickup Date | pickup_date | Body | 2 |  |   |   |
| Resolution Date | resolution_date | Body | 2 |  |   |   |
| Date Closed | close_date | Body | 2 |  |   |   |
| Performed Activities | performed_activities | Header | 12 |  |  |  |
| --- Releated Topics |  |   |  |  |   |   |
| History | history | Details | 12 | X |   |   |
| Owner Name | ownername | Header | 4 |  | X | X |

* Activity Type : Design, Development (default), Document, Testing, Other

### Hotfix {#hotfix}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |   |  |  |  |  |
| Title | title | head | 9 | X |  |  |
| Status | status | Body | 3 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| System | system | Details | 6 | X |  |  |
| ~~Nature~~ | ~~nature~~ | ~~Details~~ | ~~4~~ | ~~X~~ |  |  |
| Owner | owner | Details | 4 | (X) |  |  |
| Environments | environment | Body | 4 |  |  |  |
| --- Release Details |  |  |  |  |  |  |
| Found in | found_in | Header | 4 |  |  |  |
| Release Version | release_version | Header | 4 |  |  |  |
| Release | release | Header | 4 |  |  |  |
| --- Timing Details |  |   |  |  |  |  |
| Due Date | due_date | Body | 2 |  |  |  |
| Date Opened | open_date | Body | 2 | (X) |  |  |
| Pickup Date | pickup_date | Body | 2 |  |  |  |
| Resolution Date | resolution_date | Body | 2 |  |  |  |
| Date Closed | close_date | Body | 2 |  |  |  |
| --- Changeset Detais |  |  |  |  |  |  |
| Revisions | revisiones | Details | 6 |  |  |  |
| Files | ficheros | Details | 6 |  |  |  |
| SQL Files | sql_files | Details | 6 |  |  |  |
| Documentation | ficheros_adjuntos | Details | 6 |  |  |  |
| --- Releated Topics |  |  |  |  |  |  |
| Tasks | hotfix_tasks | Header | 6 |  |  |  |
| History |  | Details | 12 | X |  |  |
| Owner Name | ownername | Header | 4 |  | X | X |

### Changeset {#changeset}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |   |  |  |  |  |
| Title | title | head | 9 | X |  |  |
| Status | status | Body | 3 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| System | system | Details | 6 | X |  |  |
| ~~Nature~~ | ~~nature~~ | ~~Details~~ | ~~4~~ | ~~X~~ |  |  |
| Owner | owner | Details | 4 | (X) |  |  |
| Environments | environment | Body | 4 |  |  |  |
| --- Timing Details |  |   |  |  |  |  |
| Due Date | due_date | Body | 2 |  |  |  |
| Date Opened | open_date | Body | 2 | (X) |  |  |
| Pickup Date | pickup_date | Body | 2 |  |  |  |
| Resolution Date | resolution_date | Body | 2 |  |  |  |
| Date Closed | close_date | Body | 2 |  |  |  |
| ‘--- Changeset Detais |  |  |  |  |  |  |
| Revisions | revisiones | Details | 6 |  |  |  |
| Files | ficheros | Details | 6 |  |  |  |
| SQL Files | sql_files | Details | 6 |  |  |  |
| Documentation | ficheros_adjuntos | Details | 6 |  |  |  |
| --- Related Topics |  |  |  |  |  |  |
| Release | release | Header | 6 |  |  |  |
| User Stories | changeset_user_story | Header | 12 |  |  |  |
| Defects | changeset_defect | Header | 12 |  |  |  |
| History |  | Details | 12 | X |  |  |
| Owner Name | ownername | Header | 4 |  | X | X |
|  |  |  |  |  |  |  |

### Release {#release}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |   |  |  |  |  |
| Title | title | head | 8 | X |  |  |
| Status | status | Body | 4 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| ~~System~~ | ~~system~~ | ~~Details~~ | ~~4~~ | ~~X~~ |  |  |
| ~~Nature~~ | ~~Nature~~ | ~~Details~~ | ~~8~~ | ~~X~~ |  |  |
| Owner | owner | Details | 4 | (X) |  |  |
| Start Date | start_date | Body | 4 |  |  |  |
| PIP Date | fecha_prevista_pap | Body | 4 |  |  |  |
| Approval Requests | approval_requests | Header | 12 |  |  |  |
| --- Release Details |  |  |  |  |  |  |
| Previous Release | previous_release | Header | 4 |  |  |  |
| Release Version | release_version | Header | 4 |  |  |  |
| Changesets | release_changeset | Header | 12 |  |  |  |
| Hotfixes | release_hotfix | Header | 12 |  |  |  |
| Changesets Status |  |  |  |  |  |  |
| Hotfixes Status |  |  |  |  |  |  |
| --- Timing Details |  |   |  |  |  |  |
| Due Date | due_date | Body | 2 |  |  |  |
| Date Opened | open_date | Body | 2 | (X) |  |  |
| Pickup Date | pickup_date | Body | 2 |  |  |  |
| Resolution Date | resolution_date | Body | 2 |  |  |  |
| Date Closed | close_date | Body | 2 |  |  |  |
| --- Environment Details |  |  |  |  |  |  |
| Environment Plan | environment_plan | Header | 12 |  |  |  |
| Environment Requests | release_environment_request | Header | 12 |  |  |  |
| --- Related Topics |  |  |  |  |  |  |
| Documentation | ficheros_adjuntos | Header | 12 |  | X |  |
| History | history | Header | 12 | X |  |  |
| Owner Name | ownername | Header | 4 |  | X | X |

### Environment Request {#environment-request}

| Field |  | Section | Width | Mandatory | HVM | HEM |
| --- | --- | --- | --- | --- | --- | --- |
| --- Generic Information |  |   |  |  |  |  |
| Title | title | head | 9 | X |  |  |
| Status | status | Body | 3 | X |  |  |
| Description | description | Header | 12 | X |  |  |
| Owner | owner | Details | 4 | (X) |  |  |
| Release | release | Header | 4 |  |  |  |
| Environment | environment | Body | 4 |  |  |  |
| Start Date | start_date | Body | 4 |  |  |  |
| End Date | end_date | Details | 4 |  |  |  |
| Owner Name | ownername | Header | 4 |  | X | X |
| Rejection Reason | reject_reason | Header | 12 |  |  |  |