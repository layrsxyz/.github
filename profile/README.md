<div align="center">

<img alt="Layrs" src="https://raw.githubusercontent.com/layrsxyz/public/main/layrs-icon.png" width="120">

### Privacy-First Yield & Prediction Markets

*ZK-powered yield vaults and confidential trading infrastructure*

[![Website](https://img.shields.io/badge/Website-layrs.xyz-blue)](https://layrs.xyz)
[![Whitepaper](https://img.shields.io/badge/Whitepaper-Read-green)](https://github.com/layrsxyz/public/blob/main/TECHNICAL_WHITEPAPER.md)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://github.com/layrsxyz/layrs/blob/main/LICENSE)

</div>

---

## 🎯 The Problem

Most prediction markets force an impossible choice: **privacy or functionality**.

- **Polymarket** processes billions in volume → every trade is public
- **Privacy-focused alternatives** sacrifice liquidity and capital efficiency  
- **Nobody** has figured out leverage with real privacy guarantees

Users are left exposed. Professional traders avoid transparent platforms. Institutions can't participate.

## 💡 Our Solution

**Layrs** takes a fundamentally different approach:

```
Off-chain execution → Performance
Zero-knowledge proofs → Correctness  
On-chain settlement → Minimal state exposure
```

The architecture supports **up to 10x leverage with private liquidations**. When you get margin called, your position size doesn't become tradeable information.

## 🔐 Technical Architecture

### Privacy by Minimization

- **No balance leakage**: User balances never touch the chain—only cryptographic commitments
- **Withdrawal unlinkability**: Withdraw to any address, breaking the deposit→exit link
- **Private order book**: All trading activity stays off-chain

### ZEN-Denominated Liquidity

- **ERC-4626 compliant vaults** for market maker capital
- **Delta-neutral strategies** that actually work
- **Sustainable yield** for liquidity providers (80/20 fee split)

### Zero-Knowledge Proof System

| Circuit | Purpose | Status |
|---------|---------|--------|
| **User Ownership** | Prove commitment ownership without revealing identity | � Under Development |
| **Withdrawal Authorization** | Authorize withdrawals without revealing balance | 🔄 Under Development |
| **Market Resolution** | Settle positions privately when markets close | 🔄 Under Development |

**Proof aggregation** via zkVerify keeps verification costs at ~$0.0007 per proof (100x cheaper than L1 direct).

### Infrastructure

- **Horizen L3** (Base-settled) for reasonable gas costs
- **Groth16 SNARKs** (~8,000 constraints for withdrawal circuit)
- **Hub-and-spoke design** for multi-chain liquidity

## 📊 Current Status

**✅ Proof-of-Concept Validated**
- Withdrawal circuit generates valid proofs
- On-chain verification passes
- Smart contracts exist (ZKVerifier, settlement vault, liquidity vaults)

**🔄 In Progress**
- Implement user ownership circuit
- Implement market resolution circuit
- External security audits (circuits + contracts)
- Full system integration testing

**📈 Next Milestones**
- Complete remaining ZK circuits
- External audits from specialized firms
- Production hardening (multi-oracle, decentralization path)
- Capability-driven progression (no arbitrary timelines)

## 🌍 Market Opportunity

**$100B+ TAM** across:
- Sports betting
- Political forecasting  
- Crypto derivatives
- **Privacy-enabled leverage markets** (greenfield territory)

Without privacy, institutional capital stays away. With privacy, everything changes.

## 📚 Learn More

<table>
<tr>
<td width="50%">

### 📖 Documentation
- [**Technical Whitepaper**](https://github.com/layrsxyz/public/blob/main/TECHNICAL_WHITEPAPER.md) - Deep architecture dive
- [**Withdrawal Circuit**](https://github.com/layrsxyz/layrs/blob/main/docs/WITHDRAWAL_CIRCUIT.md) - Circuit technical details
- [**ZK Architecture**](https://github.com/layrsxyz/layrs/blob/main/docs/ZK_ARCHITECTURE.md) - System design overview

</td>
<td width="50%">

### 💻 Repositories
- [**layrs**](https://github.com/layrsxyz/layrs) - Public ZK showcase
  - Withdrawal circuit (Circom)
  - Verification contracts (Solidity)
  - Test suite
- **Private development repo** - Full codebase

</td>
</tr>
</table>

## 🎨 Why This Matters

> **This isn't just another prediction market.**  
> It's foundational infrastructure for privacy-preserving derivatives.

The goal: prove that confidential trading can work at institutional scale without sacrificing capital efficiency. Privacy and performance aren't mutually exclusive—you just need the right architecture.

---

<div align="center">

**Building in public. Shipping with intent.**

[Website](https://layrs.xyz) • [Whitepaper](https://github.com/layrsxyz/public/blob/main/TECHNICAL_WHITEPAPER.md) • [Documentation](https://github.com/layrsxyz/layrs)

*Leveraging zero-knowledge cryptography for financial privacy*

</div>

