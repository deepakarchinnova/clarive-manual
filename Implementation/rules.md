## Rules {#rules}

### Dashboard {#dashboard}

|  | Dashboard | Dashlet | Width |
| --- | --- | --- | --- |
| 00 | Default dashboard | Business Backlog Trendline | 12 |
| 01 | Product Management | Active Product Backlog | 6 |
| 03 | Development | All Planned User Stories by App | 4 |
| 04 | Release Management | Created Delivery per Month | 8 |
| 09 | Operations | Pending environment requests | 4 |
| 11 | Release Planning | Release Calendar | 12 |
| 10 | Release Roadmap | Release Roadmap | 12 |

### Event {#event}

|  | Event | Trigger | Scope | Type |
| --- | --- | --- | --- | --- |
| 161 | Initialize fields at topic creation | event.topic.create | Projects: | Pre Online |
| 271 | Before Status Change: SAFe Topics | event.topic.change_status | Projects: | Pre Online |
| 260 | After Status Change: SAFe Topics | event.topic.change_status | Projects: | Post Online |
| 339 | After Status Change - Update Fields: SAFe Topics | event.topic.change_status | Projects: | Post Offline |
| 276 | Before Status Change: Continuous Deployment Topics | event.topic.change_status | Projects: | Pre Offline |
| 280 | After Status Change: Continuous Delivery Topics | event.topic.change_status | Projects: | Post Online |
| 281 | After Change Status - Update Fields: Continuous Delivery Topics | event.topic.change_status | Projects: | Post Offline |
| 321 | Allow deletion of topics for following statuses: New and Closed | event.topic.delete | Projects: | Pre Online |
| 355 | Create and/or link a GitHub Mirros Repository on &quot;Create CI&quot; | event.ci.create |  | Pre Online |
| 356 | Delete the GitHub Mirror Repository | event.ci.delete |  | Pre Online |
| 353 | Manage Feature Branches: SAFe Topics | event.topic.modify.field | Projects: | Post Offline |
| 364 | Manage Feature Branches: Continuous Delivery Topics | event.topic.modify.field | Projects: | Post Offline |
| 347 | Update Ownename if owner is changed | event.topic.modify.field | Projects: | Post Offline |
| 363 | Check GitRepositoy Compliance | event.ci.update |  | Pre Online |

### Form (See [3.3 Forms](forms.md)) {#form-see-3-3-forms}

### Independent (Nothing Changed) {#independent-nothing-changed}

### Pipeline {#pipeline}

|  | Pipeline |  |
| --- | --- | --- |
| 340 | MRHE Main Job Pipeline |  |
| 348 | Dummy Job Pipeline | Used when changing statuses (when all jobs are running OK then we need to change the event rules to use the MRHE Main Job Pipeline. |

### Report (No new reports are configured) {#report-no-new-reports-are-configured}

|  | Report |
| --- | --- |
|  |  |

### Web-Service {#web-service}

|  | Web-Service | Content |
| --- | --- | --- |
| 343 | Github_sync |  |

|  | Step | Content |
| --- | --- | --- |
| 1 | Start: github_sync |  |
| 2 | Get repo_name | github_repo_name |
| 3 | Repo exists in clarive | ci-&gt;GitRepository-&gt;find_one({name=&gt; $stash-&gt;{github_repo_name}}) |
| 4 | Get Repo Location | repo_location |
| 5 | Syn with github | cd ${repo_location} &amp;&amp; git fetch --all |

### Workflow (See [3.2 Statuses](statuses.md)) {#workflow-see-3-2-statuses}