# Runbook

## Restart Service

```bash
kubectl rollout restart deployment/payment-service
```

---

## Scale

```bash
kubectl scale deployment payment-service --replicas=5
```

---

## View Logs

```bash
kubectl logs POD_NAME
```

---

## Check Health

```
GET /actuator/health
```

---

## Common Operations

- Restart pod
- Rollback deployment
- Rotate secrets
- Clear cache
