# Application Services Architecture

This repository is intended to collect and keep up to date the proposals and decisions taken into the context of the Managed Application Services group.

https://architecture.bf2.dev

## Terminology cheat sheet

 - `ADR` - Architecture Decision Record - records a decision (specific to *a single* service) that *MUST be followed* in applicable circumstances. The only way to avoid it is to supersede the decision.
 - `PADR` - Platform Architecture Decision Record - records a decision (applying to *all* services) that *MUST be followed* in applicable circumstances. The only way to avoid it is to supersede the decision.
 - `AP` - Architecture Proposal - records a decision that *SHOULD be taken into consideration* in applicable circumstances. When an AP becomes generally applicable it can be promoted to ADR/PADR.

## Service Tech Leads

The current Service Tech Leads are listed in the following GH Team:

@bf2fc6cc711aee1a0c2a/service-leads

## Contributing

The process to contribute to this repository looks as follows:

1. Someone identifies the possible need for an ADR/AP/PADR
2. They open an [issue](https://github.com/bf2fc6cc711aee1a0c2a/architecture/issues)
3. One or several of the Service Tech Leads agree on opening an ADR/AP/PADR; they assign an author (likely the person from step 1, above) and use the phrase `create adr` (or `create ap`, `create padr`). 
4. A bot open and merge a PR that assigns the id for the ADR/AP/PADR, creates a draft and closes the original issue.
5. The author opens a PR with the actual content of the proposal
5. The Service Tech Leads identify the relevant stakeholders and assign the reviewers
6. The Service Tech Leads review or delegate the review of the proposal
7. After the needed rounds of comments/discussions/updates of the PR a decision is taken to either Accept the proposal or Reject it. The outcome is recorded via the ADR/AP/PADR's `status` field. In either case, one of Service Tech Leads merges the PR
