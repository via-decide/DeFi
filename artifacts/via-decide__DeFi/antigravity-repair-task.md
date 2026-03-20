Repair mode for repository via-decide/DeFi.

TARGET
Validate and repair only the files touched by the previous implementation.

TASK
Synthesize the decentralized exchange and yield protocol into ARCHITECTURE.md and generate an automated documentation site. 1. Create docs/architecture/ and a dedicated apps/docs/ workspace using Nextra/Docusaurus. 2. Draft ARCHITECTURE.md mapping smart contract flows: Router -> Pair -> StakingVault -> Governor. 3. Detail the "Gas Optimization & Yul" philosophy and storage packing schematics. 4. Document the Constant Product Formula, $O(1)$ Staking Reward math, and impermanent loss equations. 5. Detail the Threat Model, Flash Loan attack vectors, and Reentrancy guards. 6. Implement a script (forge doc) to generate the Solidity API reference directly from NatSpec comments. 7. Enforce a slither and mythril security analysis gate in the CI/CD pipeline.

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