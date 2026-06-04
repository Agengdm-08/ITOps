# Assignment Management Use Case

## Objective

Mengelola proses assignment dan re-assignment ticket kepada IT Staff yang sesuai.

---

## Actor

### IT Supervisor

- Melakukan Assignment Ticket
- Melakukan Reassignment Ticket
- Monitoring Workload Staff

### IT Staff

- Melihat Assignment
- Menerima Assignment
- Menolak Assignment

### IT Manager

- Monitoring Assignment

### Administrator

- Konfigurasi Assignment Rule

---

## Main Flow

1. Ticket baru dibuat

2. Ticket masuk queue

3. Supervisor memilih staff

4. Ticket di-assign

5. Staff menerima assignment

6. Staff mulai bekerja

---

## Alternate Flow

### Reassignment

1. Staff tidak tersedia

2. Supervisor melakukan reassignment

3. Ticket berpindah ke staff lain

---

### Auto Assignment

1. Ticket dibuat

2. Sistem membaca assignment rule

3. Sistem memilih staff

4. Ticket otomatis diassign

---

## Status

Waiting Assignment

↓

Assigned

↓

Accepted

↓

Rejected

↓

Reassigned

---

## Output

- Assignment Record
- Assignment History
- Workload Information
- Assignment Report