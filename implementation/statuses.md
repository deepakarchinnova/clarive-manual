## Statuses {#statuses}

| Status | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| Assigned | 200 |  |  |  | Generic |
| Waiting Approval | 1400 |  |  |  | Generic |
| Waiting Planning | 1450 |  |  |  | Generic |
| ToDo | 1500 |  |  |  | Generic |
| Ready for Development | 1600 |  | X | PROD | Generic |
| Development in Progress | 1650 |  | X | PRD | Generic |
| In Development | 1700 |  |  |  | Generic |
| Ready for Integration Testing | 1740 |  | X |  | Deployable |
| In Integration Testing | 1750 |  | X | DEV | Deployable |
| Ready for Quality Assurance | 1800 |  | X |  | Deployable |
| In Quality Assurance | 2000 | X | X | QA | Deployable |
| Ready for Production | 2210 | X | X |  | Deployable |
| In Production | 2220 | X | X | PROD | Deployable |
| In Progress | 2300 |  |  |  | Generic |
| Active | 2310 |  |  |  | Generic |
| Pending Impediment | 2350 |  |  |  | Generic |
| Waiting Validation | 2400 |  |  |  | Generic |
| Done | 2500 |  |  |  | Final |
| Released | 2600 |  |  |  | Final |
| Approved | 2700 |  |  |  | Final |
| Rejected | 2750 |  |  |  | Final |
| Closed | 3000 |  |  |  | Final |
| Deployment in Progress | 3400 |  |  |  | Generic |
| Error | 3500 |  |  |  | Generic |

### Product Backlog {#product-backlog}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| Active | 2400 |  |  |  | Generic |
| Closed | 3000 |  |  |  | Final |

### Sprint {#sprint}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| ToDo | 1500 |  |  |  | Generic |
| In Progress | 2300 |  |  |  | Generic |
| Done | 2500 |  |  |  | Final |

### User Story {#user-story}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| Waiting Approval | 1400 |  |  |  | Generic |
| Waiting Planning | 1450 |  |  |  | Generic |
| ToDo | 1500 |  | X |  | Generic |
| In Progress | 2300 | X |  |  | Generic |
| Pending Impediment | 2350 |  | X |  | Generic |
| Done | 2500 |  |  |  | Final |
| Released | 2600 |  |  |  | Final |
| Approved | 2700 |  |  |  | Final |
| Rejected | 2750 |  |  |  | Final |
| Closed | 3000 |  |  |  | Final |

### Task {#task}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| ToDo | 1500 |  | X |  | Generic |
| In Progress | 2300 | X |  |  | Generic |
| Pending Impediment | 2350 |  | X |  | Generic |
| Waiting Validation | 2400 |  |  |  | Generic |
| Done | 2500 |  |  |  | Final |
| Approved | 2700 |  |  |  | Final |
| Rejected | 2750 |  |  |  | Final |
| Closed | 3000 |  |  |  | Final |

### Change Set {#change-set}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| Development in Progress | 1650 |  | X | PROD | Generic |
| Ready for Integration Testing | 1740 |  | X |  | Deployable |
| In Integration Testing | 1750 |  | X | DEV | Deployable |
| Ready for Quality Assurance | 1800 | X | X |  | Deployable |
| In Quality Assurance | 2000 | X | X | QA | Deployable |
| Ready for Production | 2210 | X | X |  | Deployable |
| In Production | 2220 | X | X | PROD | Deployable |
| Released | 2600 |  |  |  | Final |
| Closed | 3000 |  |  |  | Final |

### Hotfix {#hotfix}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| Ready for Development | 1600 |  | X | PROD | Generic |
| In Development | 1700 |  | X |  | Generic |
| Ready for Quality Assurance | 1800 | X | X |  | Deployable |
| In Quality Assurance | 2000 | X | X | QA | Deployable |
| Ready for Production | 2210 | X | X |  | Deployable |
| In Production | 2220 | X | X | PROD | Deployable |
| Released | 2600 |  |  |  | Final |
| Closed | 3000 |  |  |  | Final |

### Release {#release}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| Development In Progress | 1650 | X | X | PROD | Generic |
| Ready for Production | 2210 | X | X |  | Deployable |
| In Production | 2220 | X | X | PROD | Deployable |
| Released | 2600 |  |  |  | Final |

### Environment Request {#environment-request}

| Field | Seq | Bind Release | View Tree | Environment | Type |
| --- | --- | --- | --- | --- | --- |
| New | 100 |  |  |  | Initial |
| Assigned | 200 |  |  |  | Generic |
| Approved | 2650 |  |  |  | Final |
| Rejected | 2660 |  |  |  | Final |