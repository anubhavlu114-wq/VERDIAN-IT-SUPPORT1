# Veridian IT Service Agent

A policy-grounded internal IT employee-support agent prototype created for the Aionos Agentic AI Factory assignment.

## Assignment coverage
- Understand employee issue
- Retrieve a relevant internal policy/resolution
- Ask follow-up questions when information is missing
- Resolve simple requests with safe, actionable guidance
- Escalate risky, privileged, security-sensitive, or unclear requests
- Create a structured ticket
- Show the policy source used
- Maintain a local audit trail

## Run locally

```
Open 
Domains
Registered with

https://veridian-it-service-agent--anubhavlu999.replit.app/
veridian-it-service-agent--ANUBHAVLU999.replit.app

No API key is required. This prototype uses a transparent rule-based policy router so the behavior can be demonstrated reliably in a short interview. An LLM/RAG provider can be added behind the same interface later.

## Project structure
- `index.html` — UI
- `src/app.js` — routing, follow-ups, ticketing and audit trail
- `src/styles.css` — responsive UI
- `data/policies.json` — supplied policy knowledge base
- `tests/test-cases.json` — manual evaluation cases
- `docs/ARCHITECTURE.md` — architecture and process flow
- `docs/ASSUMPTIONS.md` — assumptions and limitations
- `docs/AI_TOOLS.md` — tools used and proposed extensions

## Demo scenarios
1. Password lockout after 6 attempts → IT unlock escalation
2. Phishing email → immediate Security escalation
3. Guest Wi-Fi → self-service guidance, no ticket required
4. Contractor VPN → manager approval requirement
5. Unclear request → follow-up question and medium-priority ticket
6. Privileged admin access → human authorization required

## Security notes
- Never ask users for passwords or secrets.
- Security incidents are routed to `security@veridian-corp.example`.
- This demo stores tickets and audit events in browser `localStorage`; production should use authenticated server-side storage.
