# Deployment

## Environments

| Environment | URL |
|------------|-----|
| DEV | |
| SIT | |
| UAT | |
| PROD | |

---

## Deployment Process

1. Build
2. Unit Test
3. Docker Image
4. Push Registry
5. Deploy Kubernetes
6. Smoke Test

---

## Rollback

Rollback previous Deployment using:

```bash
kubectl rollout undo deployment/payment-service
```
