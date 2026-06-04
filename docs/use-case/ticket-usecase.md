# Ticket Management Use Case

## Objective

Mengelola permintaan layanan IT dari user sampai ticket selesai.

---

## Actor

### Employee

- Membuat Ticket
- Melihat Status Ticket
- Menambahkan Komentar
- Menutup Ticket

### IT Staff

- Melihat Assigned Ticket
- Memproses Ticket
- Mengubah Status Ticket
- Menambahkan Worklog

### IT Supervisor

- Monitoring Ticket
- Reassign Ticket
- Eskalasi Ticket

### IT Manager

- Monitoring KPI Ticket
- Monitoring SLA

### Administrator

- Konfigurasi Sistem Ticket

---

## Main Flow

1. Employee membuat ticket

2. Sistem menghasilkan nomor ticket

3. Ticket masuk ke queue

4. Supervisor melakukan assignment

5. Staff menerima assignment

6. Staff mengerjakan ticket

7. Status berubah menjadi In Progress

8. Solusi diberikan

9. User melakukan konfirmasi

10. Ticket Closed

---

## Alternate Flow

### Reassignment

1. Staff tidak dapat menangani ticket

2. Supervisor melakukan reassign

3. Ticket berpindah ke staff lain

---

### Escalation

1. SLA mendekati breach

2. Sistem membuat escalation

3. Supervisor menerima notifikasi

---

## Status

New

↓

Assigned

↓

In Progress

↓

Pending

↓

Resolved

↓

Closed

---

## Output

- Ticket Number
- Ticket History
- Ticket Assignment
- Ticket SLA
- Ticket Report