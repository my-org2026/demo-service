# API Documentation

## Base URL

```
/api/v1/payment
```

## Authentication

- OAuth2
- JWT

---

## Endpoints

### Create Payment

POST /payments

### Get Payment

GET /payments/{id}

### Refund

POST /payments/{id}/refund

### Callback

POST /callback

---

## Error Codes

| Code | Meaning |
|------|---------|
| PAYMENT_001 | Invalid request |
| PAYMENT_002 | Payment failed |
| PAYMENT_003 | Gateway timeout |
| PAYMENT_004 | Duplicate payment |
