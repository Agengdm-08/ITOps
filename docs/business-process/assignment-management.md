# Assignment Management Business Process

## Tujuan

Mengelola proses penugasan tiket kepada IT Staff yang bertanggung jawab menangani ticket.

---

## Actor

### IT Supervisor

* Melakukan Assignment Ticket
* Melakukan Reassignment Ticket
* Monitoring Assignment

### IT Staff

* Menerima Assignment
* Menangani Ticket

---

## Assignment Flow

1. Ticket dibuat oleh Employee

2. Ticket masuk ke Queue Supervisor

3. Supervisor melakukan review ticket

4. Supervisor memilih IT Staff

5. Sistem membuat assignment

6. Status ticket menjadi ASSIGNED

7. IT Staff menerima notifikasi

8. IT Staff mulai mengerjakan ticket

---

## Reassignment Flow

1. Supervisor meninjau assignment

2. Supervisor mengganti IT Staff

3. Sistem mencatat assignment history

4. Notifikasi dikirim ke IT Staff baru

---

## Assignment Status

Waiting Assignment

↓

Assigned

↓

Accepted

↓

Rejected

↓

Reassigned

## Output

* Ticket memiliki PIC
* Assignment History tersedia
* Monitoring Assignment tersedia