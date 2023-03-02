# Application Services Architecture

This repository is intended to collect and keep up to date the proposals and decisions taken into the context of the Managed Application Services group.

https://architecture.appservices.tech

## Terminology cheat sheet

 - `ADR` - Architecture Decision Record - records a decision (specific to *a single* service) that *MUST be followed* in applicable circumstances. The only way to avoid it is to supersede the decision.
 - `PADR` - Platform Architecture Decision Record - records a decision (applying to *all* services) that *MUST be followed* in applicable circumstances. The only way to avoid it is to supersede the decision.
 - `AP` - Architecture Proposal - records a decision that *SHOULD be taken into consideration* in applicable circumstances. When an AP becomes generally applicable it can be promoted to ADR/PADR.

## Service Tech Leads

The current Service Tech Leads are:

- @tombentley
- @maleck13
- @EricWittmann
- @lburgazzoli
- @danielezonca
- @emmanuelbernard

## Contributing

The process to contribute to this repository looks as follows:

1. Identify the possible need for an ADR/AP/PADR
2. Open an [issue](https://github.com/bf2fc6cc711aee1a0c2a/architecture/issues)
3. The Service Tech Leads agree on opening an ADR/AP/PADR and assign an ID to it
4. The original issue gets closed
5. A PR with the actual content of the proposal is opened
5. The Service Tech Leads identify the relevant stakeholders and assign the reviewers
6. The Service Tech Leads review or delegate the review of the proposal
7. After the needed rounds of comments/discussions/updates of the PR a decision is taken to either Merge and accept the proposal or Reject it
