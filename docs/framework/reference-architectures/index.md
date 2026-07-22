# Enterprise Reference Architecture

```mermaid
graph TD

Users --> API

API --> Microservices

Microservices --> Events

Events --> Data Platform

Data Platform --> AI

Microservices --> Observability

Microservices --> IAM

Cloud --> Kubernetes

Kubernetes --> Microservices
```
