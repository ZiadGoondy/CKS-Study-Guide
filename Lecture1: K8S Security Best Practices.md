# Kubernetes Security and CKS Content

## 1. CKS Content
```mermaid
graph TD
    A[CKS Content]
    A --> A1[Cluster Setup - 10%]
    A --> A2[Cluster Hardening - 15%]
    A --> A3[System Hardening - 15%]
    A --> A4[Minimize Microservices Vulnerabilities - 20%]
    A --> A5[Supply Chain Security - 20%]
    A --> A6[Monitoring, Logging & Runtime Security - 20%]
```

---

## 2. Kubernetes Security Best Practices
```mermaid
graph TD
    B[Kubernetes Security Best Practices]
    B --> B1[Security Principles]
    B --> B2[Kubernetes Security Categories]
    B --> B3[Best Practices]
```

---

## 3. Security Principles
```mermaid
graph TD
    P[Security Principles]
    P --> P1[Defence in Depth]
    P --> P2[Least Privilege]
    P --> P3[Limit Attack Surface]
```

---

## 4. Kubernetes Security Categories
```mermaid
graph TD
    C[Kubernetes Security Categories]
    C --> C1[Host Operating System]
    C --> C2[Cluster Security]
    C --> C3[Application Security]
```

---

## 5. Kubernetes Best Practices
### Host Operating System
```mermaid
graph TD
    BP1[Host Operating System]
    BP1 --> BP1A[K8s nodes only for Kubernetes]
    BP1 --> BP1B[Remove unused apps]
    BP1 --> BP1C[Keep everything updated]
    BP1 --> BP1D[Runtime tools like gVisor/seccomp]
    BP1 --> BP1E[Find malicious processes]
    BP1 --> BP1F[Restrict IAM/SSH access]
```

### Kubernetes Cluster Security
```mermaid
graph TD
    BP2[Cluster Security]
    BP2 --> BP2A[Secure and up-to-date components]
    BP2 --> BP2B[Restrict external access]
    BP2 --> BP2C[Authentication & Authorization]
    BP2 --> BP2D[Admission Controllers: Node Restriction, OPA]
    BP2 --> BP2E[Audit Logging & CIS Benchmarks]
    BP2 --> BP2F[Etcd Security: Encrypt/rest/restrict access]
```

### Application Security
```mermaid
graph TD
    BP3[Application Security]
    BP3 --> BP3A[Use secrets, no hardcoded credentials]
    BP3 --> BP3B[RBAC]
    BP3 --> BP3C[Container sandboxing]
    BP3 --> BP3D[Container hardening: Reduce attack surface, run as user]
    BP3 --> BP3E[Vulnerability scanning]
    BP3 --> BP3F[mTLS/Service meshes]
```

---

## 6. Complexity of Kubernetes Security
```mermaid
graph TD
    CK[Complexity of Kubernetes security]
    CK --> CK1[Combines many things]
    CK --> CK2[Dynamic environments; security must adapt]
    CK --> CK3[Attackers have the advantage]
    CK3 --> CK3A[Decide time of attack]
    CK3 --> CK3B[Pick what to attack]
```
