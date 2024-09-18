---
title: "5G-ORAN: Conflict Mitigation"
collection: "projects"
excerpt: "5G mobile networks leverage Network Function Virtualization (NFV) to offer services in the form of network slices. Each network slice is a logically isolated fragment constructed by service chaining a set of Virtual Network Functions (VNFs). The Network Repository Function (NRF) acts as a central OpenAuthorization (OAuth) 2.0 server to secure inter-VNF communications resulting in a single point of failure. Thus, we propose 5G-WAVE, a decentralized authorization framework for the 5G core by leveraging the WAVE framework and integrating it into the OpenAirInterface (OAI) 5G core. Our design relies on Side-Car Proxies (SCPs) deployed alongside individual VNFs, allowing point-to-point authorization. Each SCP acts as a WAVE engine to create entities and attestations and verify incoming service requests. We measure the authorization latency overhead for VNF registration, 5G Authentication and Key Agreement (AKA), and data session setup and observe that WAVE verification introduces 155ms overhead to HTTP transactions for decentralizing authorization. Additionally, we evaluate the scalability of 5G-WAVE by instantiating more network slices to observe 1.4x increase in latency with 10x growth in network size. We also discuss how 5G-WAVE can significantly reduce the 5G attack surface without using OAuth 2.0 while addressing several key issues of 5G standardization."
---

* Designed and implemented a decentralized authorization framework for the 5G core service access among VNFs by utilizing WAVE to eliminate the security vulnerabilities caused by a central OAuth2.0 authorization server.

* Deployed the 5G-WAVE platform on a Kubernetes cluster with OpenAirInterface (OAI) entities as 5G VNFs.
Modified the design to offload authorization among VNFs onto side-car proxies (SCPs) which enable service
access by creation and verification of WAVE attestations.

* Measured time cost based performance of service operations in 5G-WAVE in network slice deployments to
analyze latency overhead and scalability of the design with multiple slices.
---
