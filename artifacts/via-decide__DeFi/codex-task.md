You are working in repository via-decide/DeFi on branch main.

MISSION
Synthesize the decentralized exchange and yield protocol into ARCHITECTURE.md and generate an automated documentation site. 1. Create docs/architecture/ and a dedicated apps/docs/ workspace using Nextra/Docusaurus. 2. Draft ARCHITECTURE.md mapping smart contract flows: Router -> Pair -> StakingVault -> Governor. 3. Detail the "Gas Optimization & Yul" philosophy and storage packing schematics. 4. Document the Constant Product Formula, $O(1)$ Staking Reward math, and impermanent loss equations. 5. Detail the Threat Model, Flash Loan attack vectors, and Reentrancy guards. 6. Implement a script (forge doc) to generate the Solidity API reference directly from NatSpec comments. 7. Enforce a slither and mythril security analysis gate in the CI/CD pipeline.

CONSTRAINTS
The documentation must clearly separate mathematical theory from Solidity implementation and be rigorous enough for external auditing firms (like Trail of Bits) to use as a primary reference.

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