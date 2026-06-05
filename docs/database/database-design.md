# ITOps Database Design

## Objective

Mendefinisikan struktur database yang digunakan oleh sistem ITOps berdasarkan ERD dan kebutuhan bisnis yang telah ditetapkan.

---

## Database Modules

### User Management

* roles
* users

### Ticket Management

* tickets
* ticket_comments
* ticket_worklogs

### Assignment Management

* assignments
* assignment_histories

### SLA Management

* sla_policies
* sla_logs

### Escalation Management

* escalations

### Incident Management

* incidents

### Problem Management

* problems
* known_errors

### Knowledge Base Management

* knowledge_categories
* knowledge_articles

### Notification Management

* notifications
* notification_logs

### Reporting

* reports

---

## Total Tables

16 Tables

---

## Table Definition

### roles

Purpose:

Menyimpan seluruh role yang digunakan pada sistem ITOps.

Primary Key:

* id

Referenced By:

* users.role_id

Relationship:

roles (1) ---- (N) users

Output:

* Employee
* IT Staff
* IT Supervisor
* IT Manager
* Administrator

### users

Purpose:

Menyimpan seluruh pengguna sistem ITOps.

Primary Key:

* id

Foreign Key:

* role_id → roles.id

Relationship:

roles (1) ---- (N) users

users (1) ---- (N) tickets

users (1) ---- (N) assignments

users (1) ---- (N) notifications

users (1) ---- (N) knowledge_articles

users (1) ---- (N) reports

Output:

* Employee
* IT Staff
* IT Supervisor
* IT Manager
* Administrator

### tickets

Purpose:

Menyimpan seluruh ticket yang dibuat oleh pengguna sistem.

Primary Key:

* id

Foreign Key:

* user_id → users.id
* sla_policy_id → sla_policies.id

Relationship:

users (1) ---- (N) tickets

sla_policies (1) ---- (N) tickets

tickets (1) ---- (N) ticket_comments

tickets (1) ---- (N) ticket_worklogs

tickets (1) ---- (N) assignments

tickets (1) ---- (N) escalations

tickets (1) ---- (N) incidents

Output:

* Service Request
* Incident Ticket
* Ticket History
* Ticket Status

### ticket_comments

Purpose:

Menyimpan komentar dan komunikasi pada ticket.

Primary Key:

* id

Foreign Key:

* ticket_id → tickets.id
* user_id → users.id

Relationship:

tickets (1) ---- (N) ticket_comments

users (1) ---- (N) ticket_comments

Output:

* User Comment
* Staff Comment
* Resolution Comment

### ticket_worklogs

Purpose:

Menyimpan aktivitas pengerjaan ticket oleh IT Staff.

Primary Key:

* id

Foreign Key:

* ticket_id → tickets.id
* user_id → users.id

Relationship:

tickets (1) ---- (N) ticket_worklogs

users (1) ---- (N) ticket_worklogs

Output:

* Investigation Activity
* Troubleshooting Activity
* Resolution Activity
* Work History

### assignments

Purpose:

Menyimpan penugasan ticket kepada IT Staff yang bertanggung jawab menangani ticket.

Primary Key:

* id

Foreign Key:

* ticket_id → tickets.id
* user_id → users.id

Relationship:

tickets (1) ---- (N) assignments

users (1) ---- (N) assignments

assignments (1) ---- (N) assignment_histories

Output:

* Ticket Assignment
* Assigned Staff
* Assignment Status
* Assignment Tracking

### assignment_histories

Purpose:

Menyimpan riwayat perubahan assignment ticket.

Primary Key:

* id

Foreign Key:

* assignment_id → assignments.id
* user_id → users.id

Relationship:

assignments (1) ---- (N) assignment_histories

users (1) ---- (N) assignment_histories

Output:

* Assignment History
* Reassignment History
* Assignment Audit Trail

### sla_policies

Purpose:

Menyimpan kebijakan dan aturan SLA yang digunakan pada sistem ITOps.

Primary Key:

* id

Referenced By:

* tickets.sla_policy_id
* sla_logs.sla_policy_id

Relationship:

sla_policies (1) ---- (N) tickets

sla_policies (1) ---- (N) sla_logs

Output:

* SLA Policy
* SLA Rule
* Response Time Target
* Resolution Time Target

### sla_logs

Purpose:

Menyimpan hasil perhitungan SLA untuk setiap ticket.

Primary Key:

* id

Foreign Key:

* ticket_id → tickets.id
* sla_policy_id → sla_policies.id

Relationship:

tickets (1) ---- (N) sla_logs

sla_policies (1) ---- (N) sla_logs

Output:

* SLA Timer
* SLA Achievement
* SLA Breach
* SLA History

### escalations

Purpose:

Menyimpan seluruh proses escalation ticket berdasarkan pelanggaran SLA atau kebutuhan penanganan level lebih tinggi.

Primary Key:

* id

Foreign Key:

* ticket_id → tickets.id

Relationship:

tickets (1) ---- (N) escalations

Output:

* Escalation Level 1
* Escalation Level 2
* Escalation Level 3
* Escalation History
* Escalation Monitoring

### incidents

Purpose:

Menyimpan seluruh data incident yang terjadi pada layanan dan infrastruktur IT.

Primary Key:

* id

Foreign Key:

* ticket_id → tickets.id

Relationship:

tickets (1) ---- (N) incidents

incidents (1) ---- (N) problems

Output:

* Incident Record
* Incident Severity
* Major Incident
* Incident Timeline
* Incident History
* Incident Report

### problems

Purpose:

Menyimpan data problem yang dibuat berdasarkan incident berulang atau incident yang membutuhkan analisis akar penyebab.

Primary Key:

* id

Foreign Key:

* incident_id → incidents.id

Relationship:

incidents (1) ---- (N) problems

problems (1) ---- (N) known_errors

Output:

* Problem Record
* Root Cause Analysis
* Problem History
* Problem Trend
* Problem Report

### known_errors

Purpose:

Menyimpan known error dan workaround yang ditemukan dari hasil investigasi problem.

Primary Key:

* id

Foreign Key:

* problem_id → problems.id

Relationship:

problems (1) ---- (N) known_errors

Output:

* Known Error Database
* Workaround
* Temporary Solution
* Error Reference

### knowledge_categories

Purpose:

Menyimpan kategori artikel Knowledge Base yang digunakan dalam sistem ITOps.

Primary Key:

* id

Referenced By:

* knowledge_articles.category_id

Relationship:

knowledge_categories (1) ---- (N) knowledge_articles

Output:

* Account
* Email
* VPN
* Printer
* Network
* Application
* Server
* Security

### knowledge_articles

Purpose:

Menyimpan artikel Knowledge Base yang digunakan sebagai referensi penyelesaian masalah dan panduan layanan IT.

Primary Key:

* id

Foreign Key:

* category_id → knowledge_categories.id
* user_id → users.id

Relationship:

knowledge_categories (1) ---- (N) knowledge_articles

users (1) ---- (N) knowledge_articles

Output:

* Knowledge Article
* Article Version
* Article Rating
* Article View
* Knowledge Report

### notifications

Purpose:

Menyimpan seluruh notifikasi yang dikirim oleh sistem ITOps kepada pengguna.

Primary Key:

* id

Foreign Key:

* user_id → users.id

Relationship:

users (1) ---- (N) notifications

notifications (1) ---- (N) notification_logs

Output:

* Ticket Notification
* Assignment Notification
* SLA Notification
* Escalation Notification
* Incident Notification
* Problem Notification
* Knowledge Notification

### notification_logs

Purpose:

Menyimpan histori pengiriman notifikasi dan status pengiriman.

Primary Key:

* id

Foreign Key:

* notification_id → notifications.id

Relationship:

notifications (1) ---- (N) notification_logs

Output:

* Notification History
* Delivery Report
* Delivery Status
* Retry History

### reports

Purpose:

Menyimpan data report dan hasil rekapitulasi yang digunakan untuk monitoring, dashboard, KPI, dan kebutuhan manajemen.

Primary Key:

* id

Foreign Key:

* user_id → users.id

Relationship:

users (1) ---- (N) reports

Output:

* Ticket Report
* SLA Report
* Escalation Report
* Incident Report
* Problem Report
* Knowledge Report
* KPI Report
* Management Report