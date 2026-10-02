<h1 align="center">Nader Yasser</h1>

<p align="center">
  <b>Backend &amp; full-stack developer</b> · Django · ERPNext · Laravel · AI products in Arabic
</p>

<p align="center">
  I build multi-tenant SaaS platforms and AI assistants — and run them in production myself.
</p>

<p align="center">
  <a href="mailto:naderyasser023@gmail.com"><img src="https://img.shields.io/badge/Email-naderyasser023%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://linkedin.com/in/naderyasser"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://twitter.com/naderyasser023"><img src="https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white" alt="X"></a>
  <img src="https://img.shields.io/badge/Open%20to-Freelance%20%26%20contracts-2ea44f?style=for-the-badge" alt="Open to freelance">
</p>

---

## What I do

I take products from an empty repo to a live service with paying users — schema, API, UI, AI,
servers, monitoring — and I keep them running.

- **Multi-tenant SaaS and ERP** — one codebase serving many customers, each on its own subdomain, with plans, limits, billing, accounting and an operator console.
- **AI that answers from sources** — RAG pipelines and tool-calling agents in Arabic, measured with evaluation sets instead of guessed.
- **Production I own** — Docker, Nginx, PostgreSQL, Redis, Celery and CI/CD on a VPS that hosts 40 live sites, with zero-downtime deploys.
- **Tested** — the platforms below ship with thousands of automated tests, security cases included.

---

## Selected work

Every project below has a longer write-up in **[case-studies](https://github.com/naderyasser/case-studies)**.

### SaaS & AI

#### [White-label Learning Platforms — el3aref.com](https://el3aref.com)
Education SaaS for teachers in Egypt: a teacher signs up and gets a complete learning platform on
their own subdomain within minutes — protected video courses, timed exams, printed access codes,
online and transfer payments, centre attendance, parent reports and an AI study assistant.

- Schema-per-tenant with **django-tenants**, plan limits, trials, subscriptions and an operator console (Next.js)
- Encrypted HLS video with per-viewer keys, view limits and download-tool detection
- AI study assistant with hybrid RAG over the syllabus + web search, quota per platform
- **≈93k lines of Python · 2,200+ automated tests · CI deploys with no downtime**

`Django` `DRF` `PostgreSQL` `Redis` `Celery` `Next.js` `Cloudflare R2` `Docker` · **[Full case study →](https://github.com/naderyasser/case-studies/blob/main/01-learning-platforms-saas.md)**

<a href="https://github.com/naderyasser/case-studies/blob/main/01-learning-platforms-saas.md"><img src="https://raw.githubusercontent.com/naderyasser/case-studies/main/images/learning-platform-home.png" width="640" alt="Al-Aref"></a>

#### [AI Customs Import Advisor](https://customs.educore.software)
Ask "can I import product X?" in plain Arabic and get the HS code, required approvals, bans,
duties and documents — **from official sources only, with citations**. The model is not allowed to
answer from memory: every code, approval and rate must come from a tool call in the same
conversation, and the server checks that before saving the answer.

`Python` `RAG` `Tool calling` `Embeddings` `Evaluation sets` · **[Full case study →](https://github.com/naderyasser/case-studies/blob/main/02-customs-import-advisor.md)**

<a href="https://github.com/naderyasser/case-studies/blob/main/02-customs-import-advisor.md"><img src="https://raw.githubusercontent.com/naderyasser/case-studies/main/images/customs-advisor.png" width="640" alt="Al-Aref"></a>

### ERP & business systems

#### Multi-tenant Business ERP — HR · Inventory · Sales · Accounting · POS
One platform serving many companies, each on its own subdomain with its own branding: HR and
payroll, biometric attendance, inventory, sales, purchases, accounting, a cashier (POS) and tasks —
plus a REGA-compliant real-estate marketplace built on the same core.

`Frappe / ERPNext` `Next.js` `React` `TypeScript` `Multi-tenant` · **[Full case study →](https://github.com/naderyasser/case-studies/blob/main/04-business-erp.md)**

#### Property Management for Saudi Real Estate
The full rental lifecycle in one system: properties, contracts (create, renew, terminate),
**ZATCA-compliant tax invoices** with QR codes and Arabic PDFs, Hijri dates, partial payments by
cash, transfer or cheque, and tenant accounts.

`Arabic RTL` `ZATCA` `Hijri calendar` `PDF` `PostgreSQL` · **[Full case study →](https://github.com/naderyasser/case-studies/blob/main/05-property-management.md)**

#### Multi-branch Gym ERP + members' app
Members, subscriptions, check-ins, branches, staff, finance, sales targets, bookings, recurring
payments and WhatsApp/SMS/push — plus a gamification engine and an automated retention CRM.
Three repositories: backend, staff dashboard and a members' PWA.

- **≈36.5k lines of Python across 16 Django apps · 1,200+ tests · ≈16k lines of React/TypeScript**

`Django` `React` `TypeScript` `PWA` `PostgreSQL` · **[Full case study →](https://github.com/naderyasser/case-studies/blob/main/03-gym-erp.md)**

#### [Education Centre Management (Bedaya)](https://github.com/naderyasser/SYSeducore)
Back office for tutoring centres: student files with barcode ID cards, group timetables that
detect room clashes, attendance by scanning a code, monthly fees with teacher settlements,
automatic WhatsApp reminders, and attendance/finance reports. **982 automated tests.**

`Django 5` `DRF` `PostgreSQL` `Redis` `Celery` `PWA` · **[Full case study →](https://github.com/naderyasser/case-studies/blob/main/06-education-centre.md)**

#### [Biometric Attendance — desktop edition](https://github.com/naderyasser/meena-time)
A one-time-purchase Windows app with the same rules as the cloud attendance system: reads ZKTeco
fingerprint devices over TCP/UDP, works fully offline on a local SQLite file, and exports Excel and
PDF reports.

`Electron` `SQLite` `ZKTeco` `Excel / PDF` · **[Full case study →](https://github.com/naderyasser/case-studies/blob/main/07-attendance-desktop.md)**

### Open source

#### [django-vidlock](https://github.com/naderyasser/django-vidlock)
Lock course videos in Django: encrypted single-file HLS with rotating keys, so a downloaded video
is worth nothing without its key. Extracted from the learning platform above.

---

## Stack

**Backend** &nbsp;
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![DRF](https://img.shields.io/badge/DRF-A30000?style=flat-square&logo=django&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white)

**Frontend** &nbsp;
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**Data & AI** &nbsp;
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![ERPNext](https://img.shields.io/badge/Frappe%20%2F%20ERPNext-0089FF?style=flat-square)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-%26%20agents-6E40C9?style=flat-square)

**Infrastructure** &nbsp;
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare%20R2-F38020?style=flat-square&logo=cloudflare&logoColor=white)

---

## How I can help

- **A SaaS or an ERP from zero** — multi-tenant architecture, HR, inventory, accounting, plans and billing, deployed.
- **An AI assistant that is right** — RAG or tool-calling over your own data, in Arabic, with an evaluation set.
- **A backend for your mobile app** — JWT auth, push, payments, documented APIs.
- **Rescue and hardening** — security review, tests around the money path, performance, zero-downtime deploys.

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=naderyasser&show_icons=true&hide_border=true&theme=tokyonight&count_private=true" height="150" alt="GitHub stats">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=naderyasser&layout=compact&hide_border=true&theme=tokyonight" height="150" alt="Top languages">
</p>

<p align="center">
  <b>Have a product to build or rescue?</b><br>
  Email <a href="mailto:naderyasser023@gmail.com">naderyasser023@gmail.com</a>, or reach me through <a  <a href="https://linkedin.com/in/naderyasser">LinkedIn</a>.
</p>
