---
outline: deep
head:
  - - meta
    - property: og:title
      content: Using Light Account
  - - meta
    - name: description
      content: Using Light Account with Account Kit
  - - meta
    - property: og:description
      content: Using Light Account with Account Kit
---

# Light Account

### Secure, optimized, and extendable

In Web3, efficiency, trust, and security are non-negotiable, especially with your account. That's why we built Light Account! With Light Account, we’ve turbocharged Ethereum smart accounts, reducing gas costs and supporting ERC-1271 signatures to add portability amongst all dApps. Plus, we've got your back with ownership transfer, ensuring you're never locked into a single signer. Our benchmark results speak for themselves, giving you the confidence to use a fully audited, optimized, and [open-sourced](https://github.com/alchemyplatform/light-account) smart account solution.

### Future-Proofed with Modular 6900 Accounts:

We also built Light Account with the future in mind. Light Account is forward-compatible and upgradeable for future, more optimized versions and the upcoming modular 6900 account standard, ensuring you'll stay on the cutting edge of EVM accounts. 

### The Responsible Choice

At Alchemy, in partnership with the community, we focus on the fundamentals and build our solutions from the ground up. Your trust and safety are paramount in the new digital frontier, so ensure you and your users are backed by a thoughtful craft and standard. The future of accounts is within the Alchemy Family of Smart Accounts - Optimized, Open, and Secure.

## Using Light Account

The code snippet below demonstrates the usage of Light Account with Account Kit. It creates a Light Account and sends a `UserOperation` from it:

<!--@include: ../../getting-started.md{56,68}-->

## Details

Light Account is [audited by quantstamp](https://github.com/alchemyplatform/light-account/blob/main/Quantstamp-Audit.pdf), is gas-optimized, and compatible as a [ERC-4337](https://eips.ethereum.org/EIPS/eip-4337) smart account implementation.

Based on Ethereum Foundation’s canonical [SimpleAccount](https://github.com/eth-infinitism/account-abstraction/blob/develop/contracts/samples/SimpleAccount.sol) with key improvements for production app developers, Light Account:

- significantly reduce gas costs
- [ERC-1271](https://eips.ethereum.org/EIPS/eip-1271) has signature support to ensure users can sign messages, such as on OpenSea
- allows ownership transfer so that users won’t get locked into a single `Signer`

### Benchmarks

Light Account was built optimizing for the most common user flows, providing the lowest gas cost for transfers. Here is a table of Light Account benchmarked against other smart account implementations. 

| Account              | Native transfer | ERC20 transfer | Creation |
| -------------------- | --------------- | -------------- | -------- |
| Alchemy LightAccount | 100844          | 90345          | 279746   |
| Kernel v2.1-lite     | 101002          | 90321          | 230968   |
| SimpleAccount        | 101319          | 90907          | 383218   |
| Etherspot            | 103719          | 93324          | 279219   |
| Biconomy             | 104408          | 93730          | 270013   |
| Kernel v2.1          | 106460          | 96038          | 265215   |
| Kernel v2.0          | 110018          | 99622          | 339882   |

### Developer Links

- [LightAccount & Simple Account Deployment Addresses](/smart-accounts/accounts/deployment-addresses)
- [LightAccount Github Repo](https://github.com/alchemyplatform/light-account)
- [Quantstamp Audit Report](https://github.com/alchemyplatform/light-account/blob/main/Quantstamp-Audit.pdf)
