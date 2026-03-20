Repair mode for repository via-decide/DeFi.

TARGET
Validate and repair only the files touched by the previous implementation.

TASK
Implement a secure, gas-efficient Decentralized Governance (DAO) protocol called via-defi-gov using Solidity. 1. Create src/core/governance/. 2. Implement GovernanceToken.sol extending ERC20Votes to track historical voting power via checkpoints, preventing flash-loan voting attacks. 3. Create Governor.sol configuring votingDelay, votingPeriod, and quorum. 4. Implement TimelockController.sol to route all successful proposals through a mandatory 48-hour delay before execution. 5. Build the ProposalPayload.sol interface to encode target contract addresses, ETH values, and executable calldata. 6. Transfer the owner role of via-defi-core and via-defi-vaults entirely to the TimelockController.

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