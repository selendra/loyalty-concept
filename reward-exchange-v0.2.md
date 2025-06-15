# Brand-to-Brand Loyalty Rewards Exchange Protocol

**Enabling Interoperable, Tokenized Loyalty Systems Across Cambodian Businesses**
**Powered by Selendra Network**

---

## 1. Abstract

We propose a decentralized loyalty rewards exchange protocol that allows consumers to convert, merge, and trade loyalty points across different businesses. Built on the Selendra Network, the platform tokenizes off-chain loyalty points into fungible on-chain assets, enabling users to unlock real value from fragmented reward balances.

The system supports both businesses with existing loyalty programs and those without, offering either an API for tokenization or a fully managed loyalty backend. Users benefit from a gasless, Web2-like experience, while Selendra infrastructure guarantees security, transparency, and scalability. Exchange fees and a peer-to-peer point marketplace generate sustainable revenue without burdening businesses.

---

## 2. Introduction

Loyalty programs in general are fragmented and non-interoperable. Consumers accumulate points at various businesses (e.g., cafes, fashion stores, service providers) but often do not have enough at any one place to redeem them, leading to underutilization and expiration.

Businesses, especially SMEs, face challenges:

* No incentive or mechanism to support cross-brand loyalty.
* Lack of resources to adopt blockchain or advanced loyalty systems.
* Difficulty in engaging customers with low redemption value.

This protocol addresses these gaps by creating a tokenized, interoperable loyalty network with minimal business-side integration.

---

## 3. Why Brands Like Brown & Zando Should Join

### 3.1 Unlock New Customer Acquisition

Brown and Zando can reach loyal customers of other brands who now have incentive to redeem points at their stores. This enables a new revenue stream without extra marketing costs.

### 3.2 Increase Point Redemption and Customer Engagement

Higher redemption rates increase customer return frequency and satisfaction while reducing point liabilities on the brand’s books.

### 3.3 Zero Operational Burden

No system changes or blockchain knowledge required. Brands can plug into our platform via API or dashboard — simple and seamless.

### 3.4 Monetize Idle Points

We buy points in bulk, turning unused loyalty points into real revenue for businesses.

### 3.5 First-Mover Advantage

Early adopters like Brown and Zando become pioneers in Cambodia’s first cross-brand loyalty ecosystem.

### 3.6 Access to Ecosystem Data

Gain insights into user behavior across the ecosystem that would otherwise be unavailable in isolated loyalty systems.

---

## 4. System Overview

### Key Components:

* **Tokenized Loyalty Points**: Points from businesses are mirrored on-chain using `LPoint20` tokens.
* **Swap Engine**: Users can convert points from one brand to another.
* **Point Marketplace**: Users can buy/sell loyalty tokens with others.
* **Zero-Gas UX**: All transactions are sponsored via Selendra’s gasless infrastructure or SEL token airdrops.
* **Flexible Business Integration**: For businesses with or without an existing loyalty system.
* **Point Liquidity Clearinghouse**: The platform buys and holds point reserves to facilitate cross-brand swaps without requiring bilateral business agreements.

---

## 5. Technical Design

### 5.1 Token Model

Each business has its own tokenized loyalty asset:

* Standard: `LPoint20` (ERC20-style)
* Metadata: Brand name, expiry date, redemption rate, transferability
* Managed minting and redemption rights

**Current Point Value Mapping:**

* 1 Brown Point = \$0.01 (1 cent)
* 1 Zando Point = \$0.15 (15 cents)

### 5.2 Swap Contract

* Smart contract enabling 1:1 or variable exchange between different `LPoint20` tokens.
* Supports:

  * Fixed swap rates
  * Dynamic swap routing
  * Slippage control

### 5.3 Marketplace Contract

* Peer-to-peer listing of loyalty tokens.
* Users can:

  * Sell unused points
  * Purchase points at a discount
* Fees collected in SEL or stable token.

### 5.4 Wallet & Identity

* Wallet abstraction (Web3Auth or similar)
* Login via phone/Gmail/Telegram
* Non-custodial key generation
* Users see token balances and swap history in a Web2 interface

### 5.5 Business Integration Layer

| Business Type   | Integration Path        | Notes                                 |
| --------------- | ----------------------- | ------------------------------------- |
| Existing system | API sync                | Tokenize and sync point balances      |
| No system       | Full loyalty backend    | White-labeled loyalty system provided |
| Low-tech (SMEs) | Dashboard/manual upload | CSV import or admin panel             |

---

## 6. Incentive Design & Monetization

### Revenue Streams:

* **Swap Fee**: 1–3% per point exchange (paid by user)
* **Marketplace Fee**: 5–10% per point sale
* **Premium Business Tier** *(Optional)*: Analytics, featured placement
* **Point Reserve Arbitrage**: Platform purchases points at a discount and fulfills redemptions from inventory.

### SEL Token Utility:

* Gas sponsorship for core actions
* SEL required for advanced user actions
* Airdropped SEL as user onboarding reward
* SEL staking to support point liquidity vaults and earn platform revenue

---

## 7. Point Clearinghouse Model

### Concept:

To eliminate cross-liability among businesses, the platform acts as a **clearinghouse**, buying and holding point reserves from each brand.

### How It Works:

1. **Acquire points** from businesses at negotiated rates (e.g., 80–90% of face value).
2. **User swaps** from Brand A to Brand B → Platform burns Brand A tokens, credits user Brand B tokens from reserve.
3. **Price engine** sets fair conversion rates based on token value, availability, and margin.

### Example:

* User swaps 100 Zando Points (\$15) to Brown Points (\$0.01 each)
* Platform gives 1,400 Brown Points (adjusted)
* Platform pays \$11.20 for those 1,400 points
* User pays \$12.00 or 120 SEL → platform profit: \$0.80

### Benefits:

* No need for business-to-business token acceptance
* Controlled risk via point inventory
* Direct monetization from margin and spread

---

## 8. Security & Fraud Prevention

* Authenticated business-side minting
* Signature-based redemption verification
* Reconciliation layer for off-chain vs on-chain balance
* Optional expiration and recall policies
* Liquidity vault transparency for point backing

---

## 9. Roadmap

| Phase   | Focus                 | Key Deliverables                               |
| ------- | --------------------- | ---------------------------------------------- |
| Phase 1 | MVP Pilot             | Manual tokenization for Brown & Zando          |
| Phase 2 | Swap Engine           | Deploy smart contracts, enable fixed swaps     |
| Phase 3 | Point Marketplace     | Peer listings, pricing UI, buy/sell features   |
| Phase 4 | SDK & Loyalty Builder | Tools for full system creation and analytics   |
| Phase 5 | Point Clearinghouse   | Launch reserve management & arbitrage model    |
| Phase 6 | Scale & Monetize      | 50+ businesses onboarded, SEL usage incentives |

---

## 10. Future Partners Pipeline (Top 50 Cambodian Brands)

### Food & Beverage

* Brown Coffee
* Amazon Cafe Cambodia
* KOI Thé
* Chatime Cambodia
* Tous Les Jours
* Starbucks Cambodia
* Gong Cha Cambodia
* Café Amazon
* The Pizza Company
* Lotteria Cambodia

### Fashion & Lifestyle

* Zando
* Levi’s Cambodia
* Adidas Cambodia
* Nike Cambodia
* H\&M Cambodia
* Mango Cambodia
* Puma Cambodia
* Bodia Cambodia
* Paragon Department Store
* City Mall Department Store

### Health & Wellness

* Mekong Pharmacy
* UCare Pharmacy
* Guardian Cambodia
* Doreimi Beauty Store
* Angkor Spa

### Groceries & Convenience

* Aeon Mall
* Lucky Supermarket
* Bayon Market
* Makro Cambodia
* Super Duper

### Entertainment & Leisure

* Major Cineplex Cambodia
* Legend Cinema
* Kids City
* Urban Space
* Noro Mall

### Services & Tech

* Wing Bank
* ABA Bank (loyalty partners)
* Cellcard
* Smart Axiata
* Metfone

### Travel & Lifestyle

* Cambodia Angkor Air
* PassApp
* Grab Cambodia
* Dara Hotels
* Sokha Hotels & Resorts

---

## 11. Conclusion

The Loyalty Rewards Exchange Protocol transforms fragmented, underutilized loyalty points into a dynamic, tradable asset layer. By offering tokenized, gasless transactions and a clearinghouse model, we allow users to fully redeem their accumulated value while giving businesses access to broader customer flows without operational complexity.

Powered by Selendra Network, this system is positioned to become Cambodia’s national loyalty infrastructure and a showcase model for decentralized consumer incentive systems globally.

---
