# Notification Management Use Case

## Objective

Mengelola pengiriman notifikasi sistem kepada user berdasarkan event yang terjadi pada aplikasi ITOps.

---

## Actor

### Employee

- Menerima Notifikasi
- Membaca Notifikasi

### IT Staff

- Menerima Assignment Notification
- Menerima SLA Warning

### IT Supervisor

- Menerima Escalation Notification
- Menerima SLA Breach Notification

### IT Manager

- Menerima Major Incident Notification
- Menerima KPI Notification

### Administrator

- Mengelola Notification Template
- Mengelola Notification Channel

---

## Main Flow

1. Event terjadi

2. Sistem mendeteksi event

3. Template notifikasi dipilih

4. Penerima ditentukan

5. Notifikasi dibuat

6. Notifikasi dikirim

7. User membaca notifikasi

---

## Alternate Flow

### Notification Failed

1. Pengiriman gagal

2. Sistem mencatat error

3. Sistem melakukan retry

4. Notifikasi berhasil dikirim

---

### Notification Expired

1. Notifikasi tidak dibaca

2. Notifikasi kedaluwarsa

3. Sistem melakukan archive

---

## Notification Type

### Ticket

- Ticket Created
- Ticket Assigned
- Ticket Updated
- Ticket Resolved
- Ticket Closed

### Assignment

- Assignment Created
- Assignment Reassigned
- Assignment Accepted
- Assignment Rejected

### SLA

- SLA Warning
- SLA Breach

### Escalation

- Escalation Level 1
- Escalation Level 2
- Escalation Level 3

### Incident

- Incident Created
- Incident Updated
- Incident Resolved
- Major Incident Declared

### Problem

- Problem Created
- Root Cause Identified
- Known Error Created
- Problem Resolved

### Knowledge Base

- Article Submitted
- Article Approved
- Article Published
- Article Archived

---

## Notification Channel

- In App
- Email
- Telegram

---

## Status

Pending

↓

Sent

↓

Delivered

↓

Read

↓

Archived

---

## Output

- Notification
- Notification Template
- Notification History
- Notification Log
- Delivery Report
- Email Notification
- In App Notification
- Telegram Notification