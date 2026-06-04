# ITOps Role Matrix

## Roles

1. Employee
2. IT Staff
3. IT Supervisor
4. IT Manager
5. Administrator

---

## Ticket Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| Create Ticket | Y | N | N | N | Y |
| View Own Ticket | Y | N | N | N | Y |
| View All Ticket | N | Y | Y | Y | Y |
| Update Ticket | N | Y | Y | N | Y |
| Close Ticket | N | Y | Y | N | Y |

---

## Assignment Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| View Assignment | N | Y | Y | Y | Y |
| Assign Ticket | N | N | Y | N | Y |
| Reassign Ticket | N | N | Y | Y | Y |

---

## Dashboard

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| Employee Dashboard | Y | N | N | N | Y |
| Staff Dashboard | N | Y | N | N | Y |
| Supervisor Dashboard | N | N | Y | N | Y |
| Manager Dashboard | N | N | N | Y | Y |

---

## SLA Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| View SLA | Y | Y | Y | Y | Y |
| Create SLA Policy | N | N | Y | N | Y |
| Update SLA Policy | N | N | Y | N | Y |
| View SLA Achievement | N | Y | Y | Y | Y |
| View SLA Breach | N | Y | Y | Y | Y |

---

## Escalation Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| View Escalation | N | Y | Y | Y | Y |
| Create Escalation | N | N | Y | N | Y |
| Handle Escalation | N | Y | Y | Y | Y |
| Reassign Escalation | N | N | Y | Y | Y |
| View Escalation Report | N | N | Y | Y | Y |

---

## Incident Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| Create Incident | Y | Y | Y | N | Y |
| View Incident | Y | Y | Y | Y | Y |
| Update Incident | N | Y | Y | N | Y |
| Resolve Incident | N | Y | Y | N | Y |
| Manage Major Incident | N | N | Y | Y | Y |

---

## Problem Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| View Problem | N | Y | Y | Y | Y |
| Create Problem | N | Y | Y | N | Y |
| Update Problem | N | Y | Y | N | Y |
| Approve Root Cause | N | N | Y | N | Y |
| View Problem Report | N | N | Y | Y | Y |

---

## Knowledge Base Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| View Article | Y | Y | Y | Y | Y |
| Create Article | N | Y | Y | N | Y |
| Update Article | N | Y | Y | N | Y |
| Approve Article | N | N | Y | N | Y |
| Publish Article | N | N | Y | N | Y |
| Archive Article | N | Y | Y | N | Y |

---

## Notification Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| View Notification | Y | Y | Y | Y | Y |
| Send Notification | N | N | N | N | Y |
| Manage Template | N | N | N | N | Y |
| Manage Channel | N | N | N | N | Y |
| View Notification Log | N | N | Y | Y | Y |

---

## System Administration

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| Manage User | N | N | N | N | Y |
| Manage Role | N | N | N | N | Y |
| Manage Permission | N | N | N | N | Y |
| Manage Master Data | N | N | N | N | Y |
| Manage System Configuration | N | N | N | N | Y |