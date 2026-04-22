# 🌍 Peerly v1.0

> **Connect. Learn. Explore the World.**
> A verified global student knowledge exchange platform for ages 13-19.

![Status](https://img.shields.io/badge/Status-Active_Development-brightgreen)
![Version](https://img.shields.io/badge/Version-2.0-blue)
![Confidential](https://img.shields.io/badge/Confidential-Internal_Only-red)

## 📖 Table of Contents
- [About the Project](#about-the-project)
- [Core Features](#core-features)
- [Architecture & Tech Stack](#architecture--tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Documentation](#documentation)
- [License & Confidentiality](#license--confidentiality)

## 🚀 About the Project

Peerly bridges the knowledge and cultural gap between students across different countries by enabling peer-to-peer learning, cultural exchange, and academic collaboration — all within a safe, school-verified environment.

**Core Mission:** Connect students worldwide so that every student has something to teach and something to learn — depending on where they are from.

### The Problem
- **Knowledge Asymmetry:** Students in developing countries often lack access to quality tech education and global exposure, while students in Western countries often lack exposure to diverse cultures.
- **Lack of Trust:** Existing platforms (LinkedIn, Discord, Reddit) are not designed for student-to-student exchange and carry no school-level trust layer or age-appropriate safety.

### The Solution
A school-verified social ecosystem built around:
- **Explore:** A live world map showing schools and students across every country.
- **Discover:** A smart filter system to find students by topic, country, and availability.
- **Connect:** A social feed, direct messaging, and school profile pages for ongoing relationships.

## ✨ Core Features

- **Strict User Lifecycle:** Accounts are actively available for ages 13-19. Upon turning 19, accounts automatically transition to a read-only Alumni status to maintain platform safety and relevance.
- **School-Verified Environment:** Schools are manually verified and added by Super Admins. Students can only join under verified schools.
- **Simplified RBAC:** Only two unified roles: `STUDENT` (including School Page Managers) and `SUPER_ADMIN`.
- **Safety First:** Automated image scanning (AWS Rekognition), text moderation, PII blocking, and strike-based reporting.

## 🛠 Architecture & Tech Stack

Peerly is built as a highly scalable modern web application using a monorepo architecture. 

**Frontend:**
- [Next.js](https://nextjs.org/) (App Router)
- [Tailwind CSS](https://tailwindcss.com/)
- [Mapbox GL JS](https://www.mapbox.com/) for the Explore Map

**Backend:**
- [Node.js](https://nodejs.org/) + [Express](https://expressjs.com/)
- [Zod](https://zod.dev/) for data validation
- [PostgreSQL](https://www.postgresql.org/) with [Prisma ORM](https://www.prisma.io/)
- [Redis](https://redis.io/) for caching & session management

**Infrastructure & Services:**
- Auth: Custom JWT (Access/Refresh token rotation)
- File Storage: Cloudflare R2
- Moderation: AWS Rekognition

## 🔒 License & Confidentiality
**CONFIDENTIAL**
Prepared by the Peerly Core Team. This repository and its contents are strictly confidential and proprietary. Unauthorized copying, distribution, or modification is strictly prohibited.
