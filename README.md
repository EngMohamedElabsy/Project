# 🎓 Internship Aggregator Platform

[![GitHub Issues](https://img.shields.io/github/issues/EngMohamedElabsy/Project?color=blue)](https://github.com/EngMohamedElabsy/Project/issues)
[![GitHub PRs](https://img.shields.io/github/issues-pr/EngMohamedElabsy/Project?color=green)](https://github.com/EngMohamedElabsy/Project/pulls)
[![Project Board](https://img.shields.io/badge/Board-Project%20Kanban-orange)](https://github.com/users/EngMohamedElabsy/projects/3)

A centralized software engineering platform designed to connect university students with relevant company internships and training opportunities. Built following modern Agile/Scrum requirement engineering standards and software engineering best practices.

---

## 📌 Problem & Solution Overview

### ❓ The Problem
Every year, university students face significant hurdles searching for internship opportunities scattered across fragmented social media groups, university bulletin boards, and various job portals. Students struggle to track their application statuses, while employers find it tedious to manage and filter high volumes of applicants manually.

### 💡 The Solution
A unified, transparent aggregator platform that provides:
1. **For Students:** Personalized search tailored to skills, one-click resume application, and real-time status tracking.
2. **For Employers:** A centralized dashboard to publish internships, evaluate student applicants, and streamline accept/reject decisions.
3. **For Admins:** Platform moderation to suspend spam or unverified employer accounts and track platform health metrics.

---

## 👥 User Roles

* 👨‍🎓 **Student:** Creates an account, manages profile details, searches and applies for internships, and tracks application status.
* 🏢 **Employer:** Posts new internship listings, reviews applicant profiles/resumes, and updates applicant decisions (Accept/Reject).
* 🛡️ **Admin:** Moderates user accounts, deactivates spam/fraudulent listings, and reviews platform analytics reports.

---

## 📋 User Stories & MoSCoW Prioritization Matrix

All requirements are systematically engineered and mapped to dedicated GitHub Issues:

| ID | User Story | Priority | GitHub Issue |
|:---:|:---|:---:|:---:|
| **US-01** | Student Account Registration | **Should** | [#1](https://github.com/EngMohamedElabsy/Project/issues/1) |
| **US-02** | User Profile Management | **Could** | [#2](https://github.com/EngMohamedElabsy/Project/issues/2) |
| **US-03** | Password Reset Link | **Must (MVP)** | [#3](https://github.com/EngMohamedElabsy/Project/issues/3) |
| **US-04** | Secure User Login | **Must (MVP)** | [#5](https://github.com/EngMohamedElabsy/Project/issues/5) |
| **US-05** | Search Internships by Title / Company | **Must (MVP)** | [#6](https://github.com/EngMohamedElabsy/Project/issues/6) |
| **US-06** | Apply for Internship via Profile | **Must (MVP)** | [#7](https://github.com/EngMohamedElabsy/Project/issues/7) |
| **US-07** | Post New Internship Opportunity | **Must (MVP)** | [#8](https://github.com/EngMohamedElabsy/Project/issues/8) |
| **US-08** | Review Student Applications List | **Should** | [#9](https://github.com/EngMohamedElabsy/Project/issues/9) |
| **US-09** | Update Application Status (Accept / Reject) | **Must (MVP)** | [#10](https://github.com/EngMohamedElabsy/Project/issues/10) |
| **US-10** | Track Application Status | **Should** | [#11](https://github.com/EngMohamedElabsy/Project/issues/11) |
| **US-11** | Deactivate Spam Employer Accounts | **Should** | [#12](https://github.com/EngMohamedElabsy/Project/issues/12) |
| **US-12** | Active Internships Growth Report | **Could** | [#13](https://github.com/EngMohamedElabsy/Project/issues/13) |

---

## 🚀 Minimum Viable Product (MVP Scope)

The MVP is scoped strictly to enable an end-to-end core recruitment workflow:
* **MVP Core Stories:** `US-03`, `US-04`, `US-05`, `US-06`, `US-07`, `US-09`.
* **Mandatory MVP NFR:** `NFR-02` (Password hashing using bcrypt with cost factor >= 12).
* **Rationale:** This set allows employers to publish opportunities, students to search and apply securely, and employers to render hiring decisions. Remaining Should and Could stories stay prioritized in the project backlog.

---

## 📐 Acceptance Criteria & Quality Standards

* Each user story is backed by strict **Gherkin BDD** scenarios (`Given / When / Then`).
* Detailed Non-Functional Requirements (Performance, Security, Usability, Availability) and the full Requirements Specification are maintained in [`docs/requirements.md`](docs/requirements.md).

---

## 📊 Project Kanban Board

Development progress is tracked live on the GitHub Project Board:
👉 [**Internship Platform Board**](https://github.com/users/EngMohamedElabsy/projects/3)
* 🔵 **To Do:** Prioritized backlog items.
* 🟡 **To Program:** User stories currently under development.
* 🟢 **Done:** Completed and verified user stories.

---

## 👨‍💻 Author & Maintainer
* **Mohamed Elabsy** - [@EngMohamedElabsy](https://github.com/EngMohamedElabsy)
