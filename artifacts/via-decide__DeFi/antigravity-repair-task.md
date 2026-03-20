Repair mode for repository via-decide/DeFi.

TARGET
Validate and repair only the files touched by the previous implementation.

TASK
Implement a gas-efficient Yield Farming and Staking Vault system called via-defi-vaults using Solidity. 1. Create src/core/yield/. 2. Implement StakingVault.sol to accept LP tokens and issue receipt tokens (vLP). 3. Create RewardDistributor.sol to drip a secondary governance token to stakers. 4. Implement an $O(1)$ reward accounting system using a global rewardPerTokenStored accumulator. 5. Build a TimeLock.sol module applying a multiplier to reward rates for fixed-duration locks (e.g., 30/60/90 days). 6. Implement strict ReentrancyGuard modifiers using the Checks-Effects-Interactions pattern.

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