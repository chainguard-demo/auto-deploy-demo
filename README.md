## CVE Fix and Auto-Deploy Demo

This demo walks through a full software supply chain flow:

1.	Start with a vulnerable image (Python 3.12.11 with outdated OpenSSL)
2.	Detect vulnerabilities
3.	Detect a Chainguard SLA-driven update
4.	Upgrade to Python 3.12.12
5.	Confirm the OpenSSL vulnerability was fixed within 1 Day and 15 Hours
6.	Only continue if vulnerabilities were actually removed
7.	Sign the image
8.	Attach a vulnerability attestation
9.	Deploy to Kubernetes
10.	Kyverno enforces policy at admission

Demonstrates zero-trust image promotion and policy-driven enforcement

![Alt Text](assets/pr-image.png)