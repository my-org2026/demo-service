# Payment Service

## Overview

Payment Service chịu trách nhiệm xử lý các giao dịch thanh toán của hệ thống.

Các chức năng chính:

- Tạo giao dịch thanh toán
- Kiểm tra trạng thái giao dịch
- Nhận callback từ Payment Gateway
- Hoàn tiền (Refund)
- Đối soát giao dịch

---

## Responsibilities

- Quản lý Payment Transaction
- Tích hợp Payment Gateway
- Đảm bảo tính nhất quán giao dịch
- Audit Log

---

## Technology Stack

| Component | Technology |
|-----------|------------|
| Language | Java 21 |
| Framework | Spring Boot |
| Database | PostgreSQL |
| Cache | Redis |
| Messaging | Kafka |
| Container | Docker |
| Orchestration | Kubernetes |

---

## Related Services

- Customer Service
- Order Service
- Notification Service
- Ledger Service

---

## Useful Links

- Source Code
- API Documentation
- Grafana Dashboard
- Runbook
