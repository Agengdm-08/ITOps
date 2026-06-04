# Problem Management Use Case

## Objective

Mengelola akar penyebab (Root Cause) dari incident yang berulang agar tidak terjadi kembali.

---

## Actor

### IT Staff

- Investigasi Problem
- Analisis Root Cause
- Membuat Workaround

### IT Supervisor

- Review Problem
- Menyetujui Root Cause
- Menugaskan Investigasi

### IT Manager

- Monitoring Problem KPI
- Monitoring Known Error

### Administrator

- Konfigurasi Problem Category

---

## Main Flow

1. Incident berulang terjadi

2. Problem dibuat

3. Staff melakukan investigasi

4. Root Cause ditemukan

5. Workaround dibuat

6. Known Error dibuat

7. Permanent Fix direncanakan

8. Problem ditutup

---

## Alternate Flow

### Root Cause Tidak Ditemukan

1. Investigasi dilakukan

2. Penyebab belum ditemukan

3. Problem tetap open

4. Investigasi dilanjutkan

---

### Permanent Fix

1. Root Cause ditemukan

2. RFC dibuat

3. Change dilakukan

4. Problem ditutup

---

## Problem Status

Open

↓

Under Investigation

↓

Known Error

↓

Pending Fix

↓

Resolved

↓

Closed

---

## Output

- Problem Record
- Root Cause Analysis
- Known Error
- Workaround
- Problem Report