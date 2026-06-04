# Notification Management Business Process

## Tujuan

Mengirimkan informasi secara otomatis kepada user dan tim IT berdasarkan event yang terjadi di dalam sistem.

---

## Actor

### Employee

- Menerima Notifikasi
- Membaca Notifikasi

### IT Staff

- Menerima Notifikasi Ticket
- Menerima Notifikasi SLA
- Menerima Notifikasi Incident

### IT Supervisor

- Monitoring Notification
- Monitoring Escalation Notification

### IT Manager

- Monitoring Critical Notification

### Administrator

- Mengelola Notification Template
- Mengelola Notification Channel

---

## Notification Channel

- In App
- Email
- Telegram

---

## Notification Event

### Ticket Event

- Ticket Created
- Ticket Assigned
- Ticket Updated
- Ticket Resolved
- Ticket Closed

### Assignment Event

- Assignment Created
- Assignment Reassigned
- Assignment Accepted
- Assignment Rejected

### SLA Event

- SLA Warning
- SLA Breach

### Escalation Event

- Escalation Level 1
- Escalation Level 2
- Escalation Level 3

### Incident Event

- Incident Created
- Incident Updated
- Incident Resolved
- Major Incident Declared

### Problem Event

- Problem Created
- Root Cause Identified
- Known Error Created
- Problem Resolved

### Knowledge Event

- Article Submitted
- Article Approved
- Article Published
- Article Archived

---

## Ticket Notification Flow

1. User membuat ticket

2. Sistem membuat notification

3. Notification dikirim

4. IT Staff menerima notification

5. Ticket ditangani

---

## SLA Notification Flow

1. SLA Timer berjalan

2. Sistem mendeteksi 80% SLA

3. Warning notification dikirim

4. Sistem mendeteksi SLA Breach

5. Breach notification dikirim

---

## Incident Notification Flow

1. Incident dibuat

2. Notification dikirim

3. Tim menerima notification

4. Progress update dikirim berkala

5. Incident selesai

---

## Template Management Flow

1. Admin membuat template

2. Template disimpan

3. Sistem menggunakan template

4. Notification dikirim

---

## Output

- Notification tersedia
- Notification Template tersedia
- Notification History tersedia
- Notification Log tersedia
- Delivery Report tersedia
- Email Notification tersedia
- In App Notification tersedia
- Telegram Notification tersedia