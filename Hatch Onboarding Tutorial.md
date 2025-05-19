# Hatch Onboarding Tutorial

*Version 1: Mermaid-Enhanced*  
*Version 2: Static Visuals*

---

## Table of Contents
1. [Introduction](#introduction)
2. [Platform Navigation](#platform-navigation)
3. [Workspace Structure](#workspace-structure)
4. [Creating Safe Test Workflows](#creating-safe-test-workflows)
5. [Key Workflows Deep Dive](#key-workflows-deep-dive)
6. [Safe-Testing Best Practices](#safe-testing-best-practices)
7. [Example SMS & Email Templates](#example-sms--email-templates)
8. [Hands-On Lab Checklist](#hands-on-lab-checklist)
9. [Knowledge-Check Quiz](#knowledge-check-quiz)
10. [Further Resources](#further-resources)

> **Read Me First ↘︎**  Complete **Version 1** *or* **Version 2**—they’re identical in content, but Version 1 includes live Mermaid diagrams. If your viewer can’t render Mermaid, jump to Version 2.

---

## Version 1 — Mermaid Diagrams

### 1. Introduction

Hatch automates SMS & email touch-points so leads never slip through the cracks.  
This tutorial walks you through core concepts **in production**—with **safeguards** so you won’t accidentally ping real customers.

**Goal Outcomes**

- Navigate between HTX, STX, ETX, CTX, NTX workspaces.  
- Clone and safely test the *Speed to Lead (STL)* workflow.  
- Understand & review 7 key workflows (STL, 30-Day Nurture, Revisit, Appointment Confirmation, Sweepstakes, Shows, Events).  
- Draft messages using built-in personalization tokens.  
- Pass a 10-question quiz.

> **Exercise 1.1** – Create a personal **Test Audience**.  
> 1. **Contacts → Add Contact** → enter **your** work email & mobile.  
> 2. **Audiences → New** → Name: `Test – <Your Name>` → Filter: *Email equals your@company.com* → **Save**.  
> _Outcome: Audience size = 1_

---

### 2. Platform Navigation
```mermaid
graph TD
  A[Dashboard] -->|Click| B(Workspace Selector)
  B --> C{Choose Workspace}
  C -->|NTX| D[Board]
  C -->|STX| E[Workflows]
  C -->|ETX| F[Audiences]
  subgraph Sidebar
    D
    E
    F
  end
