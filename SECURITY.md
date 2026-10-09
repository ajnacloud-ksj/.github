# Vulnerability disclosure policy

This policy tells security researchers how to report a vulnerability in the Ajna
platform or in an App that runs on it. It applies with the Acceptable Use Policy (AUP).

## How to report

- Send the report to **security@ajna.cloud**.
- Give the affected URL or App, the steps to reproduce the problem, and the effect.
- Do not put personal data or another customer's data in the report.

## What we do

1. We acknowledge the report within 5 business days.
2. We assess the report and tell you our decision.
3. We fix confirmed vulnerabilities and tell you when the fix is live.

## Coordinated disclosure: 90 days

Do not publish details of a vulnerability until one of these occurs:

- we release a fix, or
- 90 days pass after we acknowledge the report.

If we need more time, we tell you why and agree a new date with you.

## Safe harbour

AUP §3.1 says that a test of the platform needs written permission. This policy is
that written permission for a test that obeys all of these rules:

- You act in good faith.
- You test only your own Tenant. You do not access, change or delete the data of
  another Tenant or another user.
- You do not degrade the Service. Do not do load tests, denial-of-service tests or
  spam.
- You stop and report immediately when you find access to data that is not yours.
- You keep the details confidential under the 90-day rule above.

We do not take legal action against you for a test that obeys these rules.

Other tests on your own Tenant, for example a load test, need approval. Send a request
to security@ajna.cloud 5 business days before the test. An approved test can cover
only your own Tenant. A test without permission breaks AUP §3.

## Out of scope

- Social engineering and phishing of Ajna staff or customers.
- Physical attacks.
- Reports from automatic scanners with no proof of an effect.
- AWS infrastructure. Report problems with AWS itself to AWS.
