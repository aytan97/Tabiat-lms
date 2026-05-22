# TABIAT — Learning Management System

> An ongoing full-stack LMS project built from scratch. Live at [tabiat.az](https://www.tabiat.az)

TABIAT is a learning management system I am building independently. The goal is a platform where instructors can create and publish courses, and students can enroll, learn, and track their progress — with Moodle handling the actual course delivery internally.

This project is actively in development. The current focus is connecting the course catalog frontend to Moodle for content delivery.

---

## What works right now

- Instructors can create courses with title, description, intro video, pricing, and category
- Secure video storage and streaming via Cloudflare R2 (presigned URLs, token validation)
- JWT-based authentication with role separation: student, instructor, admin
- Moodle installed and tested with a SCORM package — course section integration in progress

---

## Source code

The source code is private. If you would like to see it as part of a hiring process,
feel free to reach out at aytan.sh.aa@gmail.com and I will arrange access.

---

## Tech stack

**Frontend**
- React + TypeScript (Vite)
- Redux Toolkit & RTK Query — state management and data fetching
- Tailwind CSS — styling
- Reusable component library: CourseCard, InstructorCard, Lesson pages, ratings, inputs

**Backend**
- Node.js + Express
- MongoDB — database
- Cloudflare R2 + Workers — video storage and streaming
- JWT — authentication and role-based access
- Node Mailer — email notifications
- REST API with full Swagger documentation

**Integrations**
- Moodle LMS — installed, SCORM tested, course section integration in progress

---

## Why I built this

I wanted to work on something real rather than tutorial clones. TABIAT forced me to make actual architecture decisions — how to store and stream video securely, how to structure role-based access across different user types, how to design an API that both the frontend and a third-party system (Moodle) can work with. It is still in progress and I am learning as I build.

---
> Note: Video streaming requires Cloudflare R2 credentials. Without them, video upload and playback will not work.

---

## Live site

[tabiat.az](https://www.tabiat.az)
