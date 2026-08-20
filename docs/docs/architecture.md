# Architecture

## High Level Architecture

```text
Client
   |
API Gateway
   |
Payment Service
   |
+---------------------+
| PostgreSQL          |
| Redis               |
| Kafka               |
+---------------------+

Payment Gateway
```

## Components

### REST API

External APIs.

### Business Layer

Payment processing logic.

### Repository Layer

Database access.

### Integration Layer

- Payment Gateway
- Kafka
- Notification

## Sequence Diagram

1. Receive payment request
2. Validate request
3. Call gateway
4. Persist transaction
5. Publish event
6. Return response

```mermaid
sequenceDiagram
    autonumber
    actor Client
    participant API Gateway
    participant Loan Service
    participant Database

    Client->>API Gateway: Gửi yêu cầu khởi tạo khoản vay
    API Gateway->>Loan Service: Forward request (JWT authenticated)
    Loan Service->>Database: Lưu trạng thái hồ sơ (DRAFT)
    Database-->>Loan Service: OK
    Loan Service-->>API Gateway: Response (LoanID, Status)
    API Gateway-->>Client: 201 Created
```
