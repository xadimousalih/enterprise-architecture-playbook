# API Gateway Pattern

## Intent

Provide a single entry point for all client applications while centralizing security, routing, monitoring and governance.

---

## Problem

Without an API Gateway:

- clients call services directly
- authentication is duplicated
- monitoring is fragmented
- rate limiting is inconsistent

---

## Solution

Introduce an API Gateway between consumers and backend services.

```mermaid
flowchart LR

Client --> Gateway

Gateway --> Auth

Gateway --> ServiceA

Gateway --> ServiceB

Gateway --> ServiceC
