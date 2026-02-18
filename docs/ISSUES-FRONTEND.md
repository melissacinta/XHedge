# Frontend Issues - XHedge 🎨

This document tracks the detailed UI/UX and integration tasks for the dashboard.

---

## 🚀 Module 4: Foundation & Config (Issues FE-19 to FE-22)

### Issue #FE-19: Project Scaffold & Theme
**Priority:** Critical
**Labels:** `frontend`, `config`
**Description:** Initialize Next.js 16.1.1 app with XHedge branding.
- **Tasks:**
  - [ ] Configure `tailwind.config.ts` (Dark mode focus).
  - [ ] Setup `globals.css` colors (Deep Blue/Purple).
  - [ ] Implement `Layout` with Sidebar navigation.

### Issue #FE-20: Freighter Context
**Priority:** Critical
**Labels:** `frontend`, `wallet`
**Description:** Global wallet state management.
- **Tasks:**
  - [ ] Create `FreighterContext`.
  - [ ] Implement connection logic.
  - [ ] Auto-reconnect on refresh.

### Issue #FE-21: Stellar RPC Configuration
**Priority:** High
**Labels:** `frontend`, `config`
**Description:** Setup network connection to Soroban Futurenet/Mainnet.
- **Tasks:**
  - [ ] Create `network.ts` config file.
  - [ ] Implement `getProvider` helper.

### Issue #FE-22: Component Library Setup
**Priority:** Medium
**Labels:** `frontend`, `ui`
**Description:** Install and configure ShadcnUI/Radix.
- **Tasks:**
  - [ ] Install base components (Button, Card, Input).
  - [ ] Configure `components.json`.

---

## 💼 Module 5: Vault Interface (Issues FE-23 to FE-27)

### Issue #FE-23: Vault Overview Card
**Priority:** High
**Labels:** `frontend`, `feature`
**Description:** Display key vault metrics.
- **Tasks:**
  - [ ] Fetch `total_assets` and `total_shares`.
  - [ ] Calculate and display `Share Price`.
  - [ ] Display User's Balance.

### Issue #FE-24: Deposit Tab Logic
**Priority:** High
**Labels:** `frontend`, `interaction`
**Description:** UI and logic for depositing funds.
- **Tasks:**
  - [ ] Create Deposit Form (Input + Button).
  - [ ] Build XDR for `deposit` call.
  - [ ] Handle sign & submit flow.

### Issue #FE-25: Withdraw Tab Logic
**Priority:** High
**Labels:** `frontend`, `interaction`
**Description:** UI and logic for withdrawing funds.
- **Tasks:**
  - [ ] Create Withdraw Form.
  - [ ] Build XDR for `withdraw` call.
  - [ ] Validate sufficient balance.

### Issue #FE-26: Transaction History List
**Priority:** Medium
**Labels:** `frontend`, `data`
**Description:** Show recent user actions.
- **Tasks:**
  - [ ] Fetch events from indexer (e.g., Mercury).
  - [ ] Render list of Deposits/Withdrawals.

### Issue #FE-27: Vault APY Chart
**Priority:** Medium
**Labels:** `frontend`, `chart`
**Description:** Historical performance visualization.
- **Tasks:**
  - [ ] Integrate `recharts`.
  - [ ] Fetch historical share price data.
  - [ ] Render area chart.

---

## 📈 Module 6: Analytics & AI (Issues FE-28 to FE-30)

### Issue #FE-28: Volatility Dashboard
**Priority:** Medium
**Labels:** `frontend`, `analytics`
**Description:** Visualize the AI's risk forecast.
- **Tasks:**
  - [ ] Create `RiskChart` component.
  - [ ] Display "Current Risk Level" badge.

### Issue #FE-29: Strategy Allocation Pie
**Priority:** Low
**Labels:** `frontend`, `chart`
**Description:** Show where funds are currently deployed.
- **Tasks:**
  - [ ] Fetch current allocation from contract.
  - [ ] Render Pie Chart.

### Issue #FE-30: AI Insight Stream
**Priority:** Low
**Labels:** `frontend`, `ai`
**Description:** Text feed of AI decisions.
- **Tasks:**
  - [ ] Create scrolling log component.
  - [ ] Format "Rebalance Triggered" messages.
