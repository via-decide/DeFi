You are working in repository via-decide/DeFi on branch main.

MISSION
Implement a gas-optimized Automated Market Maker (AMM) smart contract called via-defi-core using Foundry and Solidity. 1. Create src/core/amm/. 2. Implement Pair.sol holding the reserves of two ERC-20 tokens governed by the constant product formula. 3. Create Router.sol to calculate optimal execution paths across multiple Pair contracts to minimize slippage. 4. Implement a FlashLoan.sol module allowing arbitrageurs to borrow reserves with a 0.09% fee. 5. Build TickMath.sol using highly optimized bitwise operations and Yul (inline assembly) for concentrated liquidity. 6. Write a comprehensive fuzz-testing suite in test/Pair.t.sol using Foundry to mathematically prove reserves cannot be drained.

CONSTRAINTS
Strictly avoid looping over dynamic arrays in Solidity. All state variable packing must be mathematically optimized (e.g., packing into a single 256-bit storage slot) to minimize SLOAD and SSTORE gas costs.

PROCESS (MANDATORY)
1. Read README.md and AGENTS.md before editing.
2. Audit architecture before coding. Summarize current behavior.
3. Preserve unrelated working code. Prefer additive modular changes.
4. Implement the smallest safe change set for the stated goal.
5. Run validation commands and fix discovered issues.
6. Self-review for regressions, missing env wiring, and docs drift.
7. Return complete final file contents for every modified or created file.

REPO AUDIT CONTEXT
- Description: 
- Primary language: HTML
- README snippet:
not found

- AGENTS snippet:
not found


SOP: PRE-MODIFICATION PROTOCOL (MANDATORY)
1. Adherence to Instructions: No deviations without explicit user approval.
2. Mandatory Clarification: Immediately ask if instructions are ambiguous or incomplete.
3. Proposal First: Always propose optimizations or fixes before implementing them.
4. Scope Discipline: Do not add unrequested features or modify unrelated code.
5. Vulnerability Check: Immediately flag and explain security risks.

OUTPUT REQUIREMENTS
- Include: implementation summary, checks run, risks, rollback notes.
- Generate branch + PR package.
- Keep prompts deterministic and preservation-first.