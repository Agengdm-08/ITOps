# Escalation Management Use Case

## Objective

Mengelola proses eskalasi ticket yang melewati SLA atau membutuhkan penanganan level lebih tinggi.

---

## Actor

### System

- Monitoring SLA
- Membuat Escalation

### IT Supervisor

- Melihat Escalation
- Menangani Escalation
- Reassign Ticket

### IT Manager

- Monitoring Escalation
- Menangani Major Escalation

### Administrator

- Konfigurasi Escalation Rule

---

## Main Flow

1. Ticket sedang diproses

2. SLA mendekati target

3. Sistem melakukan monitoring

4. SLA terlewati

5. Sistem membuat escalation

6. Supervisor menerima notifikasi

7. Supervisor melakukan tindakan

8. Ticket diprioritaskan

9. Ticket kembali diproses

---

## Alternate Flow

### Manual Escalation

1. Staff meminta bantuan

2. Supervisor membuat escalation

3. Ticket dipindahkan ke level lebih tinggi

---

### Major Escalation

1. Ticket berdampak besar

2. Sistem menandai major escalation

3. Manager menerima notifikasi

4. Manager mengambil alih koordinasi

---

## Escalation Level

### Level 1

Supervisor

### Level 2

Manager

### Level 3

Executive Management

---

## Status

Open

↓

Acknowledged

↓

In Progress

↓

Resolved

↓

Closed

---

## Output

- Escalation Record
- Escalation History
- Escalation Notification
- Escalation Report