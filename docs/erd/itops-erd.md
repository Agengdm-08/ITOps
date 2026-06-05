# ITOps ERD Documentation

## Objective

Mendefinisikan struktur data dan relasi antar entitas pada aplikasi ITOps sebagai dasar pembuatan database dan Laravel Migration.

---

## Core Modules

1. User Management
2. Role Management
3. Ticket Management
4. Assignment Management
5. SLA Management
6. Escalation Management
7. Incident Management
8. Problem Management
9. Knowledge Base Management
10. Notification Management
11. Dashboard & Reporting

---

## Core Entities

## Entity Count

Total Entity: 16

## Entity Relationships

### User & Role

roles (1) ---- (N) users

### Ticket Management

users (1) ---- (N) tickets

tickets (1) ---- (N) ticket_comments

tickets (1) ---- (N) ticket_worklogs

### Assignment Management

tickets (1) ---- (N) assignments

users (1) ---- (N) assignments

assignments (1) ---- (N) assignment_histories

### SLA Management

sla_policies (1) ---- (N) tickets

tickets (1) ---- (N) sla_logs

### Escalation Management

tickets (1) ---- (N) escalations

### Incident Management

tickets (1) ---- (N) incidents

### Problem Management

incidents (1) ---- (N) problems

problems (1) ---- (N) known_errors

### Knowledge Base Management

knowledge_categories (1) ---- (N) knowledge_articles

users (1) ---- (N) knowledge_articles

### Notification Management

users (1) ---- (N) notifications

notifications (1) ---- (N) notification_logs

### Reporting

users (1) ---- (N) reports


### User Management

- users
- roles

### Ticket Management

- tickets
- ticket_comments
- ticket_worklogs

### Assignment Management

- assignments
- assignment_histories

### SLA Management

- sla_policies
- sla_logs

### Escalation Management

- escalations

### Incident Management

- incidents

### Problem Management

- problems
- known_errors

### Knowledge Base Management

- knowledge_articles
- knowledge_categories

### Notification Management

- notifications
- notification_logs

### Dashboard & Reporting

- reports