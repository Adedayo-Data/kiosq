# 🏪 Kiosq

> **AI-Powered Escrow & Chat Commerce Middleware for Informal Vendors**

Kiosq bridges the trust and liquidity gap in African social commerce (WhatsApp, Instagram, and direct messaging). It combines AI-driven price negotiation with a bulletproof three-party escrow model to protect buyers, empower vendors, and secure suppliers.

---

## 🚀 The Problem

Informal social commerce suffers from a severe "chicken-and-egg" liquidity problem:

1. **Trust Deficit:** Buyers are afraid of paying upfront to unverified social media vendors.
2. **Working Capital Trap:** Vendors often lack the upfront liquidity to procure goods from suppliers until the buyer pays, leading to stalled transactions and lost sales.

## 💡 The Kiosq Solution

Kiosq replaces awkward manual negotiations and risky direct bank transfers with a seamless infrastructure layer:

- **🤖 AI Bargain Portal:** An intelligent, low-friction web link shared directly in chat. An AI agent handles polite, floor-price-enforced haggling on behalf of the vendor.
- **🔒 3-Party Escrow State Machine:** Funds are locked in escrow and automatically split upon successful delivery—protecting the buyer's inspection rights, the vendor's profit margin, and the supplier's wholesale cost.
- **📦 Transit-Aware Logistics:** Automated inspection windows (e.g., 24 hours local, 48 hours interstate) backed by dual-OTP handoff verification.

---

## 🛠️ Architecture & Tech Stack

Kiosq is built as a robust, production-grade modular system:

- **Backend:** Java Spring Boot (REST APIs, Escrow State Machine, Payment Routing Logic, AI Orchestration)
- **Frontend:** React (Vite), Tailwind CSS (Mobile-first dynamic web views for bargaining and dashboards)
- **Database & Storage:** PostgreSQL / Neon, MinIO / Cloudinary for media assets
- **Integration:** Payment gateways and extensible messaging/checkout rails

---

## 📂 Project Structure

```text
kiosq/
├── backend/                  # Java Spring Boot Service (Escrow & Logic)
│   ├── src/main/java/com/kiosq/
│   │   ├── controller/       # API Endpoints (Negotiations, Escrow, Orders)
│   │   ├── model/            # Entities & State Machine definitions
│   │   └── service/          # Business logic & payment splitting
│   └── pom.xml
├── frontend/                 # React + Vite Client Application
│   ├── src/
│   │   ├── components/       # Seller Upload, Buyer Bargain Portal, Dashboard
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
└── README.md
```
