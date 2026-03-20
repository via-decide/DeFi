You are working in repository via-decide/DeFi on branch main.

MISSION
Implement a gas-efficient Yield Farming and Staking Vault system called via-defi-vaults using Solidity. 1. Create src/core/yield/. 2. Implement StakingVault.sol to accept LP tokens and issue receipt tokens (vLP). 3. Create RewardDistributor.sol to drip a secondary governance token to stakers. 4. Implement an $O(1)$ reward accounting system using a global rewardPerTokenStored accumulator. 5. Build a TimeLock.sol module applying a multiplier to reward rates for fixed-duration locks (e.g., 30/60/90 days). 6. Implement strict ReentrancyGuard modifiers using the Checks-Effects-Interactions pattern.

CONSTRAINTS
Solidity lacks floating-point numbers. Prevent precision loss by multiplying the reward numerator by $10^{18}$ before division. Calculate rewards lazily upon claiming instead of looping through users.

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