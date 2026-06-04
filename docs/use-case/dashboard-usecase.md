# Dashboard Management Use Case

## Objective

Mengelola penyajian informasi operasional, KPI, performa layanan, dan monitoring aktivitas IT secara real-time.

---

## Actor

### Employee

* Melihat Status Ticket
* Melihat Ticket History

### IT Staff

* Melihat Assigned Ticket
* Melihat SLA Ticket
* Melihat Workload

### IT Supervisor

* Monitoring Operasional IT
* Monitoring SLA
* Monitoring Escalation
* Monitoring Incident

### IT Manager

* Monitoring KPI
* Monitoring Service Performance
* Monitoring Team Performance

### Administrator

* Konfigurasi Dashboard Widget

---

## Main Flow

1. User membuka dashboard

2. Sistem memuat data operasional

3. Sistem menghitung KPI

4. Sistem menampilkan widget dashboard

5. User melakukan monitoring

---

## Alternate Flow

### Filter Dashboard

1. User memilih periode

2. Sistem memfilter data

3. Dashboard diperbarui

---

### Export Report

1. User memilih export

2. Sistem membuat report

3. Report diunduh

---

## Dashboard Type

### Employee Dashboard

* Open Ticket
* Resolved Ticket
* Closed Ticket
* Ticket History

### IT Staff Dashboard

* Assigned Ticket
* In Progress Ticket
* Resolved Ticket
* SLA Status
* Workload

### Supervisor Dashboard

* Open Ticket
* Assigned Ticket
* SLA Achievement
* Escalation Count
* Incident Count
* Problem Count

### Manager Dashboard

* Ticket Trend
* Incident Trend
* Problem Trend
* SLA Achievement
* Team Performance
* Service Performance

---

## Output

* Dashboard
* KPI
* Widget
* Monitoring
* Report
* Export
