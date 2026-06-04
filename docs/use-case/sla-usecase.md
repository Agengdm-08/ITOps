# SLA Management Use Case

## Objective

Mengelola Service Level Agreement (SLA) untuk memastikan setiap ticket ditangani sesuai target waktu layanan.

---

## Actor

### IT Supervisor

- Membuat SLA Policy
- Mengubah SLA Policy
- Monitoring SLA

### IT Manager

- Monitoring SLA Performance
- Monitoring SLA Achievement

### Administrator

- Konfigurasi SLA System

---

## Main Flow

1. Supervisor membuat SLA Policy

2. SLA Policy disimpan

3. Ticket dibuat

4. Sistem menentukan SLA

5. SLA Timer berjalan

6. Staff mengerjakan ticket

7. Ticket selesai

8. SLA dihitung

9. SLA Achievement diperbarui

---

## Alternate Flow

### SLA Warning

1. SLA mencapai 80%

2. Sistem membuat warning

3. Staff menerima notifikasi

4. Supervisor menerima notifikasi

---

### SLA Breach

1. SLA melewati target

2. Sistem mencatat breach

3. Escalation dibuat

4. Supervisor menerima notifikasi

---

## Status

Active

↓

Warning

↓

Breach

↓

Completed

---

## SLA Type

### Incident

- Critical
- High
- Medium
- Low

### Service Request

- Critical
- High
- Medium
- Low

---

## Output

- SLA Policy
- SLA Rule
- SLA Timer
- SLA Achievement
- SLA Report
- SLA Breach Report