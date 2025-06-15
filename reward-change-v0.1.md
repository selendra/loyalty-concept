# Loyalty Rewards Exchange Protocol  
**Enabling Interoperable, Tokenized Loyalty Systems Across Cambodian Businesses**  
**Powered by Selendra Network**

---

## 1. Abstract

We propose a decentralized loyalty rewards exchange protocol that allows consumers to convert, merge, and trade loyalty points across different businesses. Built on the Selendra Network, the platform tokenizes off-chain loyalty points into fungible on-chain assets, enabling users to unlock real value from fragmented reward balances.

The system supports both businesses with existing loyalty programs and those without, offering either an API for tokenization or a fully managed loyalty backend. Users benefit from a gasless, Web2-like experience, while Selendra infrastructure guarantees security, transparency, and scalability. Exchange fees and a peer-to-peer point marketplace generate sustainable revenue without burdening businesses.

---

## 2. Introduction

Loyalty programs in Cambodia are currently fragmented and non-interoperable. Consumers accumulate points at various businesses (e.g., cafes, fashion stores, service providers) but often do not have enough at any one place to redeem them, leading to underutilization and expiration.

Businesses, especially SMEs, face challenges:
- No incentive or mechanism to support cross-brand loyalty.
- Lack of resources to adopt blockchain or advanced loyalty systems.
- Difficulty in engaging customers with low redemption value.

This protocol addresses these gaps by creating a tokenized, interoperable loyalty network with minimal business-side integration.

---

## 3. System Overview

### Key Components:
- **Tokenized Loyalty Points**: Points from businesses are mirrored on-chain using `LPoint20` tokens.
- **Swap Engine**: Users can convert points from one brand to another.
- **Point Marketplace**: Users can buy/sell loyalty tokens with others.
- **Zero-Gas UX**: All transactions are sponsored via Selendra’s gasless infrastructure or SEL token airdrops.
- **Flexible Business Integration**: For businesses with or without an existing loyalty system.

---

## 4. Technical Design

### 4.1 Token Model

Each business has its own tokenized loyalty asset:
- Standard: `LPoint20` (ERC20-style)
- Metadata: Brand name, expiry date, redemption rate, transferability
- Managed minting and redemption rights

### 4.2 Swap Contract

- Smart contract enabling 1:1 or variable exchange between different `LPoint20` tokens.
- Supports:
  - Fixed swap rates
  - Dynamic swap routing
  - Slippage control

### 4.3 Marketplace Contract

- Peer-to-peer listing of loyalty tokens.
- Users can:
  - Sell unused points
  - Purchase points at a discount
- Fees collected in SEL or stable token.

### 4.4 Wallet & Identity

- Wallet abstraction (Web3Auth or similar)
- Login via phone/Gmail/Telegram
- Non-custodial key generation
- Users see token balances and swap history in a Web2 interface

### 4.5 Business Integration Layer

| Business Type         | Integration Path         | Notes                                  |
|-----------------------|--------------------------|----------------------------------------|
| Existing system        | API sync                 | Tokenize and sync point balances       |
| No system              | Full loyalty backend     | White-labeled loyalty system provided  |
| Low-tech (SMEs)        | Dashboard/manual upload  | CSV import or admin panel              |

---

## 5. Incentive Design & Monetization

### Revenue Streams:
- **Swap Fee**: 1–3% per point exchange (paid by user)
- **Marketplace Fee**: 5–10% per point sale
- **Premium Business Tier** *(Optional)*: Analytics, featured placement

### SEL Token Utility:
- Gas sponsorship for core actions
- SEL required for advanced user actions
- Airdropped SEL as user onboarding reward

---

## 6. Security & Fraud Prevention

- Authenticated business-side minting
- Signature-based redemption verification
- Reconciliation layer for off-chain vs on-chain balance
- Optional expiration and recall policies

---

## 7. Roadmap

| Phase     | Focus                 | Key Deliverables                                 |
|-----------|------------------------|--------------------------------------------------|
| Phase 1   | MVP Pilot              | Manual tokenization for Brown & Zando           |
| Phase 2   | Swap Engine            | Deploy smart contracts, enable fixed swaps       |
| Phase 3   | Point Marketplace      | Peer listings, pricing UI, buy/sell features     |
| Phase 4   | SDK & Loyalty Builder  | Tools for full system creation and analytics     |
| Phase 5   | Scale & Monetize       | 50+ businesses onboarded, SEL usage incentives   |

---

## 8. Conclusion

The Loyalty Rewards Exchange Protocol aims to transform fragmented, underutilized loyalty points into interoperable, high-utility digital assets. By offering gasless, user-friendly access to tokenized points—and by enabling flexible business participation—the platform supports both consumers and local businesses without introducing unnecessary friction.

Built on the Selendra Network, this solution has the potential to become the loyalty infrastructure of Cambodia and beyond.

---
