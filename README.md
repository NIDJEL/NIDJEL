<div align="center">

# Nikita Kruglov

### Go Backend Engineer · Distributed Systems · High-Load Systems

I build backend and infrastructure software with Go, focusing on concurrency, networking, correctness, and systems engineering. I also contribute patches to the official Go project.

<p>
  <a href="https://go.dev/"><img alt="Go" src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&amp;logo=go&amp;logoColor=white"></a>
  <a href="https://en.cppreference.com/w/c"><img alt="C" src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&amp;logo=c&amp;logoColor=white"></a>
  <a href="https://isocpp.org/"><img alt="C++" src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&amp;logo=cplusplus&amp;logoColor=white"></a>
  <a href="https://learn.microsoft.com/dotnet/csharp/"><img alt="C#" src="https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&amp;logo=dotnet&amp;logoColor=white"></a>
  <a href="https://www.postgresql.org/"><img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&amp;logo=postgresql&amp;logoColor=white"></a>
  <a href="https://redis.io/"><img alt="Redis" src="https://img.shields.io/badge/Redis-B9292F?style=for-the-badge&amp;logo=redis&amp;logoColor=white"></a>
  <a href="https://www.docker.com/"><img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&amp;logo=docker&amp;logoColor=white"></a>
  <a href="https://aws.amazon.com/"><img alt="AWS" src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&amp;logo=amazonwebservices&amp;logoColor=FF9900"></a>
  <a href="https://kernel.org/"><img alt="Linux" src="https://img.shields.io/badge/Linux-23272A?style=for-the-badge&amp;logo=linux&amp;logoColor=FCC624"></a>
  <a href="https://git-scm.com/"><img alt="Git" src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&amp;logo=git&amp;logoColor=white"></a>
  <a href="https://github.com/"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&amp;logo=github&amp;logoColor=white"></a>
</p>

[**Merged Go contributions**](https://go-review.googlesource.com/q/owner:nikkruglov16@gmail.com+status:merged) · [**My repositories**](https://github.com/NIDJEL?tab=repositories)

</div>

---

## Open Source · Go Project Contributor

<div align="center">

<a href="https://go.dev/"><img alt="Go Project" src="https://img.shields.io/badge/Go_Project-Contributor-00ADD8?style=for-the-badge&amp;logo=go&amp;logoColor=white"></a>
<img alt="3 upstream merges" src="https://img.shields.io/badge/3-Merged_Upstream-238636?style=for-the-badge&amp;logo=git&amp;logoColor=white">
<img alt="Maintainer reviewed" src="https://img.shields.io/badge/Maintainer-Reviewed-30363D?style=for-the-badge&amp;logo=github&amp;logoColor=white">

<br>

**Accepted contributions to the official Go repositories.**  
Concurrency correctness, HTTP/2 networking, and Go build infrastructure.

</div>

<br>

### 01 · `database/sql` — Concurrency & Deadlock Prevention

<p>
  <img alt="Go Standard Library" src="https://img.shields.io/badge/Go-Standard_Library-00ADD8?style=flat-square&amp;logo=go&amp;logoColor=white">
  <img alt="Concurrency" src="https://img.shields.io/badge/Concurrency-Synchronization-6E40C9?style=flat-square">
  <img alt="Merged" src="https://img.shields.io/badge/Status-Merged_Upstream-238636?style=flat-square&amp;logo=git&amp;logoColor=white">
</p>

Fixed a **lost-wakeup race** in `closingMutex` writer coordination that could deadlock concurrent `Rows.Next` and `Rows.Close` operations. The fix corrects mutex state handling and adds regression coverage.

[**CL 820060 — View merged change ↗**](https://go-review.googlesource.com/c/go/+/820060) · [Go issue #81043](https://github.com/golang/go/issues/81043)

---

### 02 · `net/http` — HTTP/2 TLS State

<p>
  <img alt="Go Standard Library" src="https://img.shields.io/badge/Go-Standard_Library-00ADD8?style=flat-square&amp;logo=go&amp;logoColor=white">
  <img alt="HTTP/2" src="https://img.shields.io/badge/Networking-HTTP%2F2-0969DA?style=flat-square">
  <img alt="Merged" src="https://img.shields.io/badge/Status-Merged_Upstream-238636?style=flat-square&amp;logo=git&amp;logoColor=white">
</p>

Corrected the HTTP/2 server so `Request.TLS` accurately reflects the **underlying TLS connection**, including CONNECT requests and HTTP targets over TLS, with corresponding test coverage.

[**CL 829184 — View merged change ↗**](https://go-review.googlesource.com/c/go/+/829184) · [Go issue #81384](https://github.com/golang/go/issues/81384)

---

### 03 · `x/build/internal/gcsfs` — Go Infrastructure

<p>
  <img alt="Go Infrastructure" src="https://img.shields.io/badge/Go-Infrastructure-00ADD8?style=flat-square&amp;logo=go&amp;logoColor=white">
  <img alt="Google Cloud Storage" src="https://img.shields.io/badge/Google_Cloud-Storage-4285F4?style=flat-square&amp;logo=googlecloud&amp;logoColor=white">
  <img alt="Merged" src="https://img.shields.io/badge/Status-Merged_Upstream-238636?style=flat-square&amp;logo=git&amp;logoColor=white">
</p>

Fixed directory listing for **explicit Google Cloud Storage folders** represented by zero-byte marker objects, preventing phantom child entries while preserving empty-directory detection.

[**CL 828164 — View merged change ↗**](https://go-review.googlesource.com/c/build/+/828164) · [Go issue #81359](https://github.com/golang/go/issues/81359)

<div align="center">
  <a href="https://go-review.googlesource.com/q/owner:nikkruglov16@gmail.com+status:merged"><img alt="Verified merged Go contributions" src="https://img.shields.io/badge/View_Merged_Go_Contributions-Gerrit-0B1117?style=for-the-badge&amp;logo=go&amp;logoColor=00ADD8"></a>
</div>

---

## Verified AWS

<div align="center">

<a href="https://www.credly.com/badges/ed05c89f-b6ac-4e72-a2d5-eed862dd695a/public_url">
  <img
    src="assets/aws-application-networking-demonstrated.png"
    width="180"
    alt="AWS Application Networking Demonstrated"
  />
</a>

### AWS Application Networking Demonstrated

**Amazon Web Services Training and Certification Aug 2026**

Hands-on AWS assessment covering application networking, service-to-service communication, load balancing, container networking, observability, and cloud infrastructure.

<p>
  <img alt="AWS" src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&amp;logo=amazonwebservices&amp;logoColor=FF9900">
  <img alt="VPC Lattice" src="https://img.shields.io/badge/VPC_Lattice-8A2BE2?style=flat-square">
  <img alt="Amazon ECS" src="https://img.shields.io/badge/Amazon_ECS-FF9900?style=flat-square&amp;logo=amazonecs&amp;logoColor=white">
  <img alt="CloudFront" src="https://img.shields.io/badge/CloudFront-8A2BE2?style=flat-square&amp;logo=amazonwebservices&amp;logoColor=white">
  <img alt="API Gateway" src="https://img.shields.io/badge/API_Gateway-FF4F8B?style=flat-square&amp;logo=amazonapigateway&amp;logoColor=white">
  <img alt="CloudWatch" src="https://img.shields.io/badge/CloudWatch-FF4F8B?style=flat-square&amp;logo=amazoncloudwatch&amp;logoColor=white">
</p>

**[Verify credential on Credly](https://www.credly.com/badges/ed05c89f-b6ac-4e72-a2d5-eed862dd695a/public_url)**

</div>

---

## Selected Projects

### [Vless VPN](https://github.com/NIDJEL/vless-vpn) · Go / Wails / React / sing-box

Windows desktop VPN and proxy client supporting VLESS, SOCKS5, TLS/REALITY, system proxy and TUN modes, process-based split tunneling, subscription management, and connection health checks. Sensitive local configuration is protected with Windows DPAPI.

### [DentVision](https://github.com/NIDJEL/dentvision) · Go / PostgreSQL / Python / FastAPI / YOLO

Dental X-ray analysis application combining a Go REST API, PostgreSQL-backed patient and inference records, a separate Python ML service, and an interactive results interface.

### [loglint](https://github.com/NIDJEL/loglint) · Go / go/analysis / golangci-lint

Custom Go static analyzer for logging conventions and basic sensitive-data checks, with `analysistest` coverage and `golangci-lint` integration.

### [AI Scheduler](https://github.com/NIDJEL/ai-calendar) · Kotlin / Jetpack Compose / GigaChat

Android scheduling application with an LLM-based command parser and a deterministic, local scheduling engine. Calendar changes require explicit confirmation.

---

## Engineering Focus

`Concurrent Programming` · `Distributed Systems` · `Backend Architecture` · `Microservices` · `Networking` · `Databases` · `Performance Engineering` · `Reliability` · `High-Load Systems`

## Credentials

- **AWS Application Networking Demonstrated** — AWS Microcredential · **Verified on Credly**
- **IBM Developer Skills Network** — Docker Essentials: A Developer Introduction

## Current Focus

`Go Standard Library` · `Concurrency & Synchronization` · `Networking / HTTP` · `Backend Infrastructure` · `Performance & Profiling` · `Developer Tooling`
