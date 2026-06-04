# ITOps Role Matrix

## Roles

1. Employee
2. IT Staff
3. IT Supervisor
4. IT Manager
5. Administrator

---

## Ticket Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| Create Ticket | Y | N | N | N | Y |
| View Own Ticket | Y | N | N | N | Y |
| View All Ticket | N | Y | Y | Y | Y |
| Update Ticket | N | Y | Y | N | Y |
| Close Ticket | N | Y | Y | N | Y |

---

## Assignment Management

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| View Assignment | N | Y | Y | Y | Y |
| Assign Ticket | N | N | Y | N | Y |
| Reassign Ticket | N | N | Y | Y | Y |

---

## Dashboard

| Permission | Employee | Staff | Supervisor | Manager | Admin |
|------------|----------|--------|------------|---------|--------|
| Employee Dashboard | Y | N | N | N | Y |
| Staff Dashboard | N | Y | N | N | Y |
| Supervisor Dashboard | N | N | Y | N | Y |
| Manager Dashboard | N | N | N | Y | Y |