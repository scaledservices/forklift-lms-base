# forklift-lms-base

This repository contains the **base LMS template code** originally derived from the Marshal LMS tutorial project. It serves as a **foundational scaffold** for extending into a full training and certification platform.

This is *not yet* a fully customized training system; instead, it contains a functional LMS structure that supports courses, lessons, admin tools, user accounts, and payment integration foundations.

---

## Current Project Overview

This codebase is a **full-stack Learning Management System scaffold** built with:

- **Next.js (App Router)**
- **TypeScript**
- **Prisma ORM**
- **Stripe integration scaffold**
- **React UI components**

It implements basic LMS features rather than a complete, training-specific application.

### Key Capabilities (as currently implemented)

#### **Authentication**
- Email-based login pages
- Auth API routes
- Role guards using middleware

#### **Public Pages**
- Course catalog
- Landing pages
- Public UI components

#### **Admin Dashboards**
- Course creation & editing
- Lesson management
- Dashboard statistics views

#### **Learner Dashboard**
- Enrolled course list
- Lesson navigation
- Progress tracking

#### **Payments (Stripe)**
- Stripe checkout webhook route (`/api/webhook/stripe`)
- Payment success & cancel pages

#### **File Upload Support**
- S3 compatible upload/delete API endpoints
- File uploader UI components

---

## Repository Structure (High Level)

```plaintext
app/
  (auth)/        Authentication UI and routes
  (public)/      Public pages and course catalog
  admin/         Admin course/curriculum management
  dashboard/     Learner-focused course progress area
  api/           Backend logic (auth, uploads, webhooks)
components/      Shared UI components
hooks/           Reusable React hooks
lib/             Core utilities (auth, DB, Stripe, environment)
prisma/          Database schema
public/          Static assets
