# Beauty Catalyst Engine 💄
**High-Performance Beauty Catalog & Headless CMS Lead Generation System.**

[![Lighthouse Score](https://img.shields.io/badge/Lighthouse-100%2F100-brightgreen.svg)](#)
[![Framework](https://img.shields.io/badge/Architecture-Headless_CMS_/_Serverless-blue.svg)](#)
[![Data Layer](https://img.shields.io/badge/Data_Layer-Google_Sheets_API-green.svg)](#)
[![SEO](https://img.shields.io/badge/SEO-Structured_Data_Ready-orange.svg)](#)

A production-grade web engine tailored for the luxury beauty and cosmetic sector. This system implements a **Zero-Build CMS** architecture, allowing non-technical stakeholders to manage high-velocity inventory updates via Google Sheets while maintaining a blazing-fast, SEO-optimized frontend experience.

---

## 🚀 Live Production Environment
**[Explore the Interface ↗](https://demomakeup.netlify.app/)**

---

## 📸 Interface Showcase
*(Full-page architecture and UI layout)*

<p align="center">
  <img src="assets/full-page-preview.png" alt="Beauty Catalyst Engine Full Interface" width="100%">
</p>

---

## 🧠 System Architecture & Flow

To ensure maximum performance and client autonomy, the engine follows a decoupled data-fetching pattern. This allows the UI to stay light while the data remains dynamic.

```mermaid
graph LR
  A[Google Sheets CMS] -->|REST API / JSON| B(Middleware Parser)
  B -->|Dynamic Mapping| C[Frontend Interface]
  C -->|Lead Capture| D{Lead Pipeline}
  D -->|SMTP/API| E[Client Inbox]
