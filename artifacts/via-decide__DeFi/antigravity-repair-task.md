Repair mode for repository via-decide/DeFi.

TARGET
Validate and repair only the files touched by the previous implementation.

TASK
Implement a gas-optimized Automated Market Maker (AMM) smart contract called via-defi-core using Foundry and Solidity. 1. Create src/core/amm/. 2. Implement Pair.sol holding the reserves of two ERC-20 tokens governed by the constant product formula. 3. Create Router.sol to calculate optimal execution paths across multiple Pair contracts to minimize slippage. 4. Implement a FlashLoan.sol module allowing arbitrageurs to borrow reserves with a 0.09% fee. 5. Build TickMath.sol using highly optimized bitwise operations and Yul (inline assembly) for concentrated liquidity. 6. Write a comprehensive fuzz-testing suite in test/Pair.t.sol using Foundry to mathematically prove reserves cannot be drained.

RULES
1. Audit touched files first and identify regressions.
2. Preserve architecture and naming conventions.
3. Make minimal repairs only; do not expand scope.
4. Re-run checks and provide concise root-cause notes.
5. Return complete contents for changed files only.

SOP: REPAIR PROTOCOL (MANDATORY)
1. Strict Fix Only: Do not use repair mode to expand scope or add features.
2. Regression Check: Audit why previous attempt failed before proposing a fix.
3. Minimal Footprint: Only return contents for the actual repaired files.

REPO CONTEXT
- README snippet:
not found
- AGENTS snippet:
not found
- package.json snippet:
not found