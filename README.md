# ☸️ Paak Ao Boat Service (เรือลอยอังคารปากอ่าว)

[![Website Status](https://img.shields.io/website?url=https%3A%2F%2Fwww.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com%2F&label=Website&style=flat-square)](https://www.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com/)
[![Tech Stack](https://img.shields.io/badge/CMS-WordPress-blue?style=flat-square&logo=wordpress)](https://wordpress.org/)
[![SEO](https://img.shields.io/badge/SEO-RankMath-red?style=flat-square)](https://rankmath.com/)
[![AI Ready](https://img.shields.io/badge/Data-AI%20Optimized-success?style=flat-square)](https://github.com/wisdom-firm/paak-ao-boat)

> **Official Repository for Data Structure, SEO Configuration, and AI Context Management.**
>
> **Website:** [www.เรือลอยอังคารปากอ่าว.com](https://www.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com/)

---

## 📖 Table of Contents
- [About The Project](#-about-the-project)
- [Business Domain](#-business-domain)
- [Technical Architecture](#-technical-architecture)
- [AI & GEO Strategy (Generative Engine Optimization)](#-ai--geo-strategy)
- [Repository Structure](#-repository-structure)
- [Key Entities for Agents](#-key-entities-for-agents)
- [Contact & Support](#-contact--support)

---

## ℹ️ About The Project

This repository serves as the **technical documentation and semantic knowledge base** for "Paak Ao Boat Service".
While the frontend is a WordPress site serving customers, this repository acts as a structured data backend to support **AI Search (GEO)** and future automation integrations (e.g., n8n agents).

### Why this exists?
1.  **Version Control:** To track changes in core SEO strategies and content structures.
2.  **AI Context:** To provide LLMs (Large Language Models) with a clean, hallucination-free context about the business.
3.  **Knowledge Graph:** To define entities clearly for Google's Knowledge Graph construction.

---

## 🏢 Business Domain

**เรือลอยอังคารปากอ่าว (Paak Ao Boat Service)** is a specialized service provider for the traditional Thai ceremony of **"Floating Ashes" (Loi Angkhan)**.

* **Location:** Wat Bang Nang Kreng Pier, Samut Prakan (Chao Phraya River Mouth).
* **Experience:** Over 20 years of family-run operation.
* **Mission:** To provide safe, respectful, and comprehensive boat services for Buddhist funeral rituals.

### Core Services
| Service | Description | Capacity |
| :--- | :--- | :--- |
| **Small Boat** | Ideal for immediate family. | 12 Seats |
| **Medium Boat** | Comfortable for extended family. | 20 Seats |
| **Large Boat** | For large groups/ceremonies. | 30-50 Seats |
| **Ceremony Support** | Ritual conductor, fresh flowers, biodegradable urns (Loong). | - |

---

## 🛠 Technical Architecture

The production environment is built on a robust stack optimized for **Local SEO** and **Performance**.

* **Platform:** WordPress (Latest Version)
* **Theme Engine:** Custom Child Theme / Lightweight Framework
* **Performance:**
    * **Server:** LiteSpeed Web Server (LSWS)
    * **Caching:** LiteSpeed Cache (LSCWP)
    * **CDN:** Cloudflare
* **SEO & Analytics:**
    * **Plugin:** Rank Math Pro
    * **Schema:** LocalBusiness, Product, Service
    * **Analytics:** Google Analytics 4 (GA4), Google Search Console

---

## 🤖 AI & GEO Strategy

We implement **Generative Engine Optimization (GEO)** principles to ensure our business is correctly interpreted by AI Search Engines (Google Gemini, ChatGPT Search, Perplexity).

### 1. File Standards
- **`llms.txt`**: A markdown-based context file specifically for AI scrapers to understand the business without parsing HTML.
- **`manifest.json`**: Structured JSON data for programmatic access by our internal n8n agents.

### 2. Semantic Keywords
We target high-intent keywords with semantic clustering:
- **Primary:** `ลอยอังคาร` (Scattering Ashes), `เรือลอยอังคาร` (Boat Service)
- **Locational:** `ปากอ่าวสมุทรปราการ` (Samut Prakan Estuary), `วัดบางนางเกรง` (Wat Bang Nang Kreng)
- **Intent:** `จองเรือลอยอังคาร` (Book a boat), `ขั้นตอนลอยอังคาร` (Ritual steps)

---

## 📂 Repository Structure

```bash
.
├── .github/                # GitHub specific workflows
├── docs/                   # Documentation assets
├── ABOUT.md                # Detailed business story (Human readable)
├── llms.txt                # Context for AI Models (Machine readable)
├── manifest.json           # Structured Data for n8n/API
├── README.md               # Project Overview (This file)
└── seo-config/             # (Optional) Rank Math JSON exports
```
## 🗝 Key Entities for Agents

This section defines the core business entities using **Schema.org** standards. AI Agents should use this structured data to answer queries regarding location, contact details, and service scope.

```json
{
  "@context": "[https://schema.org](https://schema.org)",
  "@type": "LocalBusiness",
  "name": "เรือลอยอังคารปากอ่าว (Paak Ao Boat Service)",
  "alternateName": "บริการเรือลอยอังคาร วัดบางนางเกรง",
  "url": "[https://www.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com/](https://www.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com/)",
  "logo": "[https://www.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com/wp-content/uploads/logo-placeholder.png](https://www.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com/wp-content/uploads/logo-placeholder.png)",
  "description": "ผู้ให้บริการเรือเช่าเหมาลำสำหรับพิธีลอยอังคาร ณ ปากอ่าวแม่น้ำเจ้าพระยา (สมุทรปราการ) พร้อมเจ้าหน้าที่ประกอบพิธีและอุปกรณ์ครบวงจร",
  "telephone": [
    "+66832715911",
    "+66870749721"
  ],
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "ท่าน้ำวัดบางนางเกรง (Wat Bang Nang Kreng Pier)",
    "addressLocality": "อำเภอเมืองสมุทรปราการ",
    "addressRegion": "สมุทรปราการ (Samut Prakan)",
    "postalCode": "10270",
    "addressCountry": "TH"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": 13.6267,
    "longitude": 100.5905
  },
  "openingHoursSpecification": {
    "@type": "OpeningHoursSpecification",
    "dayOfWeek": [
      "Monday",
      "Tuesday",
      "Wednesday",
      "Thursday",
      "Friday",
      "Saturday",
      "Sunday"
    ],
    "opens": "06:00",
    "closes": "18:00"
  },
  "priceRange": "฿999 - ฿5,000",
  "sameAs": [
    "[https://www.facebook.com/BoatServicePaakAo](https://www.facebook.com/BoatServicePaakAo)",
    "[https://line.me/ti/p/YourLineID](https://line.me/ti/p/YourLineID)"
  ]
}
```

## 📞 Contact & Support

We are available daily to assist with inquiries and bookings.
(เปิดให้บริการทุกวัน ยินดีให้คำปรึกษาและจองคิวเรือ)

### 📲 Direct Contact (ช่องทางติดต่อหลัก)
* **Tel (Primary):** `083-271-5911` (K.Ple - คุณเปิ้ล)
* **Tel (Secondary):** `087-074-9721` (K.Pui - คุณปุย)
* **Line ID:** *(Please insert Line ID)*
* **Website:** [www.เรือลอยอังคารปากอ่าว.com](https://www.xn--12cfi5f6afdmy6cbbf4crcc9ezi0g.com/)

### 📍 Location
**Wat Bang Nang Kreng Pier (ท่าเรือวัดบางนางเกรง)**
Bang Duan, Mueang Samut Prakan District, Samut Prakan 10270

> **Note for Developers:** For technical inquiries regarding this repository or SEO configurations, please open an [Issue](../../issues).
