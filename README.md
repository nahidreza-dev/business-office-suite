# Business Office Suite

**One private back office for a whole agency or IT company: money, clients, quotes, invoices, projects, a shared email inbox, team roles, work time, leave and payroll.**

I designed, built and run this system for my own company, [GoAutoSiteAI](https://goautositeai.com). My team uses it every day. If you want something like this for your business, I can build one for you, made to fit the way you work.

👉 **Want one?** [nahidreza.com/contact](https://nahidreza.com/contact) · [Book a free 30-minute call](https://nahidreza.com/book)

> All screenshots use **Sample** data. Real client data, email addresses, keys and private links are never shown.
>
> The source code is kept in a private repository. Clients get their own copy, set up under their own name and accounts.

![Dashboard](screenshots/01-dashboard.jpg)

---

## What it does

### 💰 Money and reports
- Income, expenses and transfers across cash, bank and mobile wallets (bKash, Nagad), in taka and dollars.
- Recurring entries such as rent, salaries and software are added by themselves every month.
- Profit and loss by month, by category, by client and by project. Export to Excel.

### 🤝 Clients, quotes and invoices
- A client list with balance due, WhatsApp link and preferred language.
- Proposals and quotations on the company letterhead. The client opens a link and **accepts online**, and a project is created automatically.
- Invoices split into instalments (for example 40% / 30% / 30%), automatic payment reminders, a **PAID** stamp, and payments recorded straight into the books.
- Every document can be downloaded as a PDF, in **English or Bangla**, with a language switch on the page.

### 📋 Projects, support and handover
- A task board for each project (To do, Doing, In review, Done), with email notices when a task is assigned.
- Team members only see their own projects.
- Support requests with internal notes and emailed replies.
- A handover checklist that the client signs off online.

### 📥 Shared email inbox
- support@, billing@ and hello@ in one inbox, connected to the company's real mailboxes.
- Replies go out from the real address, with the person's name and the company signature.
- **Each team member sees only the mailboxes their role allows.**
- Pass an email to a colleague, mark it done, save the sender as a client, and download attachments.
- One-click delete or select-all delete, plus optional auto-clean of old emails. This only removes emails from the Office; the real mailbox is never touched.
- New mail arrives by itself within minutes.

### 👥 Team, roles and access
- Invite members with one link (short named links with a PIN are optional).
- Give access **by role**, give **everything**, or **pick each permission by hand**.
- Every action is recorded in an activity log.

### ⏱️ Work time, leave and payroll (built for flexible IT teams)
- A start/stop work timer linked to a project or task, idle detection, daily updates, team timelines and weekly reports.
- No "late" marking.
- Leave requests and approvals with yearly allowances, weekends and holidays.
- Payroll for monthly or hourly pay: works out the month, adds bonus or advance, pays into the books, and creates a payslip PDF.

### 🌐 Built for real use
- The whole interface works in **Bangla and English**.
- Light and dark mode. Works well on phones and can be **installed as an app**.
- Two-step sign-in by email code, session limits and rate limiting.

---

## Screenshots

| | |
|---|---|
| ![Reports](screenshots/03-reports.jpg) | ![Clients](screenshots/04-clients.jpg) |
| **Profit and loss** | **Clients** |
| ![Quotes](screenshots/05-quotes.jpg) | ![Invoices](screenshots/06-invoices.jpg) |
| **Proposals and quotes** | **Invoices** |
| ![Project board](screenshots/07-project-board.jpg) | ![Support](screenshots/08-support.jpg) |
| **Project task board** | **Support requests** |
| ![Inbox](screenshots/09-inbox.jpg) | ![Email thread](screenshots/10-inbox-thread.jpg) |
| **Shared email inbox** | **Reply from the real mailbox** |
| ![Work time](screenshots/11-work-time.jpg) | ![Payroll](screenshots/12-payroll.jpg) |
| **Work time** | **Payroll** |
| ![Leave](screenshots/13-leave.jpg) | ![Team](screenshots/14-team.jpg) |
| **Leave** | **Team** |
| ![Roles](screenshots/15-roles.jpg) | ![Access](screenshots/17-access-picker.jpg) |
| **Roles and access** | **Give access by role, everything, or by hand** |
| ![Letterhead](screenshots/16-letterhead.jpg) | ![Invoice PDF](screenshots/18-invoice-pdf.jpg) |
| **Company letterhead settings** | **Invoice on the letterhead** |
| ![Quote in Bangla](screenshots/19-quote-bangla.jpg) | |
| **The same quote in Bangla** | |

### On the phone

| | | |
|---|---|---|
| ![Mobile dashboard](screenshots/20-mobile-dashboard.jpg) | ![Mobile inbox](screenshots/21-mobile-inbox.jpg) | ![Mobile invoices](screenshots/22-mobile-invoices.jpg) |

---

## How it is built

- **Serverless:** runs on Cloudflare Workers with a D1 (SQL) database. There is no server to manage, and it stays fast worldwide.
- **One small app:** a single-page app written in plain JavaScript and CSS, with no heavy frameworks. It loads quickly, even on mobile data.
- **Email:** Resend for system emails. The shared inbox uses the company's own mailboxes through the Hostinger Mail API, kept in sync by webhooks and a 5-minute schedule.
- **Documents:** HTML pages on the company letterhead, ready to print or save as PDF, in Bangla and English.
- **Security:** hashed passwords (PBKDF2), HttpOnly session cookies, an optional email code at sign-in, role-based permissions checked on the server, rate limits, an audit log, and a strict sandbox for incoming email HTML.
- **Tested:** automated browser tests (Playwright) on desktop and a 390 px phone, run before every release.

---

## Want this for your business?

I build custom office systems, client dashboards and SaaS products. Each one fits your workflow, carries your brand, and runs under your own accounts.

- 🌐 [nahidreza.com](https://nahidreza.com)
- 📅 [Book a free call](https://nahidreza.com/book)
- ✉️ [Send your project details](https://nahidreza.com/contact)

**Nahid Reza**: founder of GoAutoSiteAI, based in Bangladesh, working with clients worldwide.
