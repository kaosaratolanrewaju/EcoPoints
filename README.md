# ♻️ EcoPoints — Waste into Wealth

> **A community platform that turns recycling into rewards.**  
> Built for the Kenyon Group × SPE Nigeria Council Sustainability Challenge · World Environment Day 2026.

---

## 🌍 The Problem

Nigeria generates millions of tonnes of solid waste annually, yet recycling infrastructure and community participation remain critically low. In cities like Warri and Effurun, recyclable materials — plastic, paper, metal, glass — end up in drains and open dumps, driving flooding, disease, and environmental degradation.

The barrier isn't awareness. It's incentive.

---

## 💡 Our Solution

**EcoPoints** makes sustainability tangible. Residents separate recyclable materials at home and deposit them at community collection hubs or through pickup teams. Every kilogram earns **EcoPoints** — redeemable for real-world rewards like airtime, school supplies, and transport vouchers.

Schools and neighbourhoods compete on **EcoScore leaderboards**, making environmental action a community sport. And when points are pooled together, they fund shared infrastructure — boreholes, solar streetlights, green parks — turning individual effort into collective impact.

We are not just recycling waste. We are transforming waste into wealth, and environmental action into a lifestyle.

---

## 🔑 Key Features

| Feature | Description |
|---|---|
| 📱 **QR Deposit System** | Residents scan a QR code at collection hubs to log deposits and earn points instantly |
| ⚖️ **Points Engine** | Each kilogram earns EcoPoints based on material type (plastic, paper, metal, glass) |
| 🎁 **Rewards Marketplace** | Redeem points for airtime, school supplies, transport vouchers, or food market credits |
| 🏆 **EcoScore Leaderboards** | Neighbourhood and school rankings drive friendly competition and sustained participation |
| 🌍 **Community Fund** | Pool points collectively to fund shared projects — boreholes, streetlights, green parks |
| 🏗️ **Hub Dashboard** | Admin portal for collection hub operators to track volumes, manage capacity, and view analytics |

---

## 🖥️ Live Demo

👉 **[View the Interactive Prototype →](https://your-demo-link-here.netlify.app)**

The demo includes:
- **Resident App** — QR deposit flow, points balance, rewards redemption, and personal EcoScore ranking
- **Hub Dashboard** — Collection analytics, hub status monitoring, school leaderboards, and community project progress

> _To explore: open the link, choose a portal, and interact with the full deposit-to-redeem flow._

---

## 🏗️ How It Works

```
Resident separates waste at home
        ↓
Deposits at collection hub or schedules pickup
        ↓
Hub operator scans QR / logs deposit by weight & material
        ↓
EcoPoints credited instantly to resident's mobile account
        ↓
Points redeemed for rewards  ──OR──  pooled for community projects
        ↓
School / neighbourhood EcoScore updates on leaderboard
```

---

## 📐 Technical Architecture (Proposed)

```
┌─────────────────────────────────────────────┐
│              RESIDENT MOBILE APP             │
│    QR Scanner · Points Wallet · Rewards      │
└──────────────────┬──────────────────────────┘
                   │ REST API
┌──────────────────▼──────────────────────────┐
│              BACKEND SERVICES                │
│  Points Engine · Auth · Rewards Ledger       │
│  Notification Service · Analytics           │
└────────┬──────────────────┬─────────────────┘
         │                  │
┌────────▼──────┐   ┌───────▼──────────────────┐
│   DATABASE    │   │     HUB DASHBOARD         │
│  PostgreSQL   │   │  Admin Web Portal         │
│  (Users,      │   │  Collection Tracking      │
│  Transactions,│   │  Hub Management           │
│  Rewards)     │   │  Leaderboards             │
└───────────────┘   └──────────────────────────┘
```

**Proposed tech stack:**
- **Mobile App:** React Native (Android + iOS, USSD fallback for feature phones)
- **Backend:** Node.js / Express, REST API
- **Database:** PostgreSQL
- **QR System:** Dynamic QR codes tied to hub ID + session token
- **Points Settlement:** Real-time via mobile wallet integration (Flutterwave / Paystack)
- **Rewards Fulfilment:** Airtime via VTU APIs, physical goods via partner logistics

---

## 🗺️ Rollout Plan

### Phase 1 — Pilot (Months 1–3)
- Launch 3 collection hubs in Warri/Effurun
- Onboard 2 secondary schools for EcoScore competition
- Deploy resident mobile app (Android) with QR deposit flow
- Manual rewards fulfilment (airtime top-up, supply drops)

### Phase 2 — Scale (Months 4–8)
- Expand to 10+ hubs across Delta State
- Integrate automated airtime and voucher disbursement via API
- Launch community pooling feature for infrastructure projects
- Partner with DESOPADEC and local government for co-funding

### Phase 3 — Replicate (Month 9+)
- Open-source the hub dashboard for adoption by other states
- Onboard corporate sponsors for reward top-ups (CSR integration)
- Explore USSD-based participation for non-smartphone users

---

## 🌱 Impact Targets (Year 1)

| Metric | Target |
|---|---|
| Registered residents | 5,000+ |
| Kilograms recycled | 50,000 kg |
| CO₂ equivalent offset | ~100 tonnes |
| Schools participating | 20+ |
| Community projects funded | 5 |
| Collection hubs | 15 |

---

## 👥 Team

Built by petroleum engineering students at the **Federal University of Petroleum Resources, Effurun (FUPRE)** — proving that sustainability innovation doesn't only come from tech hubs.

---

## 📄 License

MIT License — open for adaptation by other communities and sustainability initiatives.

---

> *"We are not just recycling waste. We are transforming waste into wealth and environmental action into a lifestyle."*  
> — EcoPoints Team, FUPRE
