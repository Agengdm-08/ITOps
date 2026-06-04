# Incident Management Use Case

## Objective

Mengelola gangguan layanan IT agar dapat dipulihkan secepat mungkin dan meminimalkan dampak bisnis.

---

## Actor

### Employee

- Melaporkan Incident
- Melihat Status Incident

### IT Staff

- Mencatat Incident
- Melakukan Diagnosis
- Menangani Incident
- Memulihkan Service

### IT Supervisor

- Monitoring Incident
- Mengelola Major Incident
- Koordinasi Tim

### IT Manager

- Monitoring Incident KPI
- Monitoring Major Incident

### Administrator

- Konfigurasi Incident Category

---

## Main Flow

1. User melaporkan gangguan

2. Sistem membuat incident

3. Staff menerima incident

4. Staff melakukan diagnosis

5. Penyebab ditemukan

6. Perbaikan dilakukan

7. Service dipulihkan

8. User melakukan verifikasi

9. Incident ditutup

---

## Alternate Flow

### Major Incident

1. Dampak incident sangat besar

2. Incident ditandai sebagai major

3. Supervisor menerima notifikasi

4. Tim khusus dibentuk

5. Recovery dilakukan

---

### Escalation

1. Incident tidak dapat diselesaikan

2. Incident dieskalasi

3. Supervisor melakukan koordinasi

---

## Severity

### Critical

- Service down total

### High

- Banyak user terdampak

### Medium

- Sebagian user terdampak

### Low

- Dampak kecil

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

- Incident Record
- Incident History
- Incident Report
- Incident KPI
- Major Incident Report