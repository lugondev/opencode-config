## 🐞 Debug & Troubleshooting (Web3 / DeFi)

### 🧪 Frontend Debug

* Browser DevTools (Elements, Network, Performance)
* Debug state inconsistency & re-render issues
* Memory leak detection
* Responsive & cross-browser debugging
* Mobile Safari / Chrome mobile debugging

---

### 🔗 Transaction Debug

* Full transaction lifecycle:

  * `sign → submit → pending → confirm → fail`
* Handle stuck, dropped, replaced transactions
* Decode revert reasons & custom errors
* Gas estimation & gas-related failures
* Debug approval vs execution issues

---

### 🌐 RPC & Network Issues

* RPC timeout & fallback handling
* Chain mismatch & network switching errors
* Provider instability & rate limiting
* Multi-RPC awareness
* Debug inconsistent on-chain reads

---

### 🧩 DeFi UX Debug

* Wrong balances & stale UI state
* Sync UI state with on-chain state
* Slippage & price mismatch debugging
* Race conditions between UI & blockchain
* Edge cases: paused contracts, empty pools, low liquidity

---

## 🧱 Backend & Smart Contract Debug

### 🔌 Backend / API Debug

* Debug REST / GraphQL APIs
* Frontend ↔ backend data mismatch analysis
* Signature-based authentication debugging
* Cache & eventual consistency issues
* Correlate logs between frontend, backend & tx hash

---

### 📦 Indexer & Data Layer

* Understanding of:

  * The Graph / Subgraphs
  * Custom indexers (RPC → DB)
* Debug missing or delayed events
* Handle reorgs & inconsistent indexing
* Fallback UX for indexer lag

---

### 📜 Smart Contract Debug (Frontend Perspective)

* Read & understand ABI and interfaces
* Interpret revert reasons & custom errors
* Debug permission, role & pause logic
* Validate contract state via block explorers
* Distinguish frontend vs backend vs contract bugs

---

### ⛽ Gas & Execution Debug

* Gas estimation failures
* Out-of-gas & underpriced transactions
* Simulation success but execution failure
* Nonce, replacement & cancel transaction handling

---

### 🔍 Cross-Layer Debug Workflow

* Trace issues across:

  * UI → API → RPC → Smart Contract → Events → Indexer → UI
* Compare expected vs on-chain state
* Use transaction traces & event logs
* Write clear bug reports for backend / contract teams

---

## 🔧 Tooling & Workflow

* Git / GitHub
* Vite / Webpack
* ESLint / Prettier
* PNPM / Yarn
* Figma (developer handoff & inspection)

---

## 🤝 Collaboration

* Work closely with smart contract engineers
* Collaborate with backend & protocol teams
* Understand DeFi business logic
* Agile / sprint-based development

---

## 🌱 Nice to Have

* Framer Motion / GSAP
* Storybook
* Accessibility audits
* Multi-chain UX awareness (EVM / Solana / Cosmos)

---

## 🎯 Engineering Focus

* UX safety for financial actions
* Prevent user fund loss through better UI
* Clear state over assumptions
* Defensive coding for unreliable RPCs
* Clean, maintainable, performance-aware code
