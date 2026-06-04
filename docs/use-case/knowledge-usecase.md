# Knowledge Base Management Use Case

## Objective

Mengelola artikel pengetahuan (Knowledge Article) sebagai referensi penyelesaian incident, problem, dan service request.

---

## Actor

### Employee

- Melihat Artikel
- Mencari Solusi

### IT Staff

- Membuat Artikel
- Mengubah Artikel
- Menggunakan Artikel

### IT Supervisor

- Review Artikel
- Approve Artikel
- Publish Artikel

### IT Manager

- Monitoring Knowledge KPI

### Administrator

- Konfigurasi Category

---

## Main Flow

1. Incident selesai

2. Solusi didokumentasikan

3. Artikel dibuat

4. Supervisor melakukan review

5. Artikel diapprove

6. Artikel dipublish

7. User mencari artikel

8. Artikel digunakan kembali

---

## Alternate Flow

### Artikel Ditolak

1. Artikel dibuat

2. Review dilakukan

3. Artikel ditolak

4. Artikel direvisi

5. Review ulang

---

### Artikel Update

1. Solusi berubah

2. Artikel diperbarui

3. Versi baru dibuat

4. Artikel dipublish ulang

---

## Status

Draft

↓

Review

↓

Approved

↓

Published

↓

Archived

---

## Category

### Account

- User Account
- Password Reset
- Access Management

### Email

- Email Configuration
- Email Troubleshooting
- Email Recovery

### VPN

- VPN Setup
- VPN Access
- VPN Troubleshooting

### Printer

- Printer Setup
- Printer Troubleshooting
- Printer Sharing

### Network

- Network Configuration
- Connectivity Issue
- WiFi Troubleshooting

### Application

- Application Installation
- Application Usage
- Application Troubleshooting

### Server

- Server Administration
- Server Monitoring
- Server Troubleshooting

### Security

- Security Policy
- Security Incident
- Security Awareness

---

## Output

- Knowledge Article
- Knowledge Category
- Article Version
- Article Rating
- Article View