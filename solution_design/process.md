## Process {#process}

### High-Level {#high-level}

| Topic | Application | Description | Type |
| --- | --- | --- | --- |
| Product Backlog | Clarive |  | Normal |
| HotFix | Clarive | Kanban | Changeset |
| Sprint | Clarive | Scrum | Normal |
| User Story | Clarive | Scrum | Normal |
| Defect | Clarive | Scrum | Normal |
| Task | Clarive | Scrum | Normal |
| Changeset | Clarive | Deployable | Changeset |
| Release | Clarive | Release Management | Release |

### Detailed workflows (to be implemented) {#detailed-workflows-to-be-implemented}

#### SAFe Agile workflows {#safe-agile-workflows}

Product Backlog

| From | To | Role(s) | Rule(s) |
| --- | --- | --- | --- |
| New | Active | Product Owner |  |
| Active | Closed |  |  |

Sprint

| From | To | Role(s) | Rule(s) |
| --- | --- | --- | --- |
| New | ToDo | Scrum Master |  |
| ToDo | New |  |  |
| In Progress | ToDo |  |  |

User Story

| From | To | Role(s) | Rule(s) |  |
| --- | --- | --- | --- | --- |
| New | ToDo | Product Owner |  |  |
| ToDo | Waiting Approval | (System) | Activity Type = ‘Requirement’ or ‘Design’ |  |
| Waiting Approval | Approved | Business Owner |  |  |
| Approved | Waiting Planning | (System) |  |  |
| Waiting Planning | ToDo | Srcum Master |  |  |
| ToDo | New |  |  |  |
| In Progress | ToDo |  |  |  |
| Pending Impediment | In Progress |  |  |  |
| Done | Released | (System) | Triggered when release is transitioned to status ‘Released’. |  |

Defect

| From | To | Role(s) | Rule(s) |  |
| --- | --- | --- | --- | --- |
| New | ToDo | Product Owner |  |  |
| ToDo | In Progress | Scrum Master |  |  |
| In Progress | In Progress |  |  |  |
| Waiting Impediments | In Progress |  |  |  |
| Done | Released | (System) | Triggered when release is transitioned to status ‘Released’. |  |

Task

| From | To | Role(s) | Rule(s) |  |
| --- | --- | --- | --- | --- |
| New | ToDo | Scrum Master |  |  |
| ToDo | New |  |  |  |
| In Progress | ToDo |  |  |  |
| Waiting Impediments | In Progress |  |  |  |
| Done | Waiting Validation | (System) | Activity Type = ‘Design’ |  |
| Waiting Validation | ToDo (Rejected) | Business Owner |  |  |

#### Continuous Delivery workflows {#continuous-delivery-workflows}

Changeset

| From | To | Role(s) | Rule(s) |  |
| --- | --- | --- | --- | --- |
| New | Development in Progress | Release Manager |  |  |
| Development in Progress | Ready for Integration Testing | Release Manager Developer |  |  |
| Ready for Integration Testing | In Integration Testing |  |  | Promote (DEV) |
| In Integration Testing | Ready for Quality Assurance |  |  | Demote (DEV) |
| Ready for Quality Assurance | In Quality Assurance | Release Manager |  | Promote (QA) |
| In Quality Assurance | Ready for Production | Product Owner |  | Demote (QA) |
| Ready for Production | In Production | (System) | Triggered by a Release transitional to the ‘To’-Status | Promote (PROD) |
| In Production | Released | (System) |  | Demote (PROD/QA) |

* Not Implemented

Hotfix (= Changeset with less workflow steps)

| From | To | Role(s) | Rule(s) |  |
| --- | --- | --- | --- | --- |
| New | Ready for Development | Product Owner |  |  |
| Ready for Development | In Development | Scrum Master |  |  |
| In Development | Ready for Quality Assurance |  |  |  |
| Ready for Quality Assurance | In Quality Assurance | Release Manager |  | Promote (QA) |
| In Quality Assurance | Ready for Production | Product Owner |  | Demote (QA) |
| Ready for Production | In Production | Release Manager | Can be triggered by a Release transitional to the ‘To’-Status | Promote (PROD) |
| In Production | Released | Product Owner |  | Demote (PROD/QA) |

Release

| From | To | Role(s) | Rule(s) |  |
| --- | --- | --- | --- | --- |
| New | Development in Progress | Product Owner |  |  |
| Development in Progress | Ready for Production |  |  |  |
| Ready for Production | In Production | Release Manager |  | Promote (PROD) |
| In Production | Released | Product Owner |  | Demote (PROD/QA) |

#### Supporting Workflows {#supporting-workflows}

Environment Request

| From | To | Role(s) | Rule(s) |  |
| --- | --- | --- | --- | --- |
| New | Assigned | Release Manager |  |  |
| Assigned | Approved | System Architect |  |  |