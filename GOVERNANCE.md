# Policy Labs & AMPEL Governance Document

This document defines the governance lifecycle for AMPEL and all repositories housed under the Policy Labs organization ([https://github.com/policylabs](https://github.com/policylabs)).

## 1. Governing Principles

* **Open Source First:** The project is intended to facilitate and bind together the open-source supply chain ecosystem.
* **Non-partisan:** The project should be technology and format agnostic when technically feasible. There are no winning formats or technologies.
* **Fostering Community Growth:** All decisions should mind the growth, health, and inclusivity of the community.
* **Security & Compliance by Design:** Given the project's role in the supply chain, decisions must prioritize robust software architectures and compliance-friendly workflows, ensuring downstream users can easily audit and trust the ecosystem.
* **Interoperability:** The project will strive for seamless integration with modern software delivery mechanisms, including containerized environments, signing frameworks, and diverse CI/CD pipelines.

## 2. Steering Committee (SC)

* The Policy Labs organization and its core projects shall be governed by a Steering Committee consisting of at least 3 and up to 7 members. There should always be an odd number of committee members.
* Any one organization should never control more than 1/3 of the voting seats to ensure vendor neutrality.
* The standard term of an SC member will be up to two years. Members can be reelected.
* When an SC seat opens up, an SC issue will be opened on the community site. Interested parties may self-nominate. The remaining SC members will elect a new member based on project merit and contributions. The vote to accept a new member must be unanimous.
* SC members must vote on decision points. Any SC member absent when votes take place 3 or more consecutive times may be replaced by freeing the seat and electing a new member.

## 3. Decision Making & Voting Process

* The SC will vote on major or contentious issues within the organization. Issues will be put to a vote on the community site by creating a dedicated issue.
* Large technical enhancements will require opening a special Enhancement Proposal issue to capture feedback and the formal SC vote.
* **Quorum & Timeline:** There is a minimum quorum of 33% of the SC members to reach a binding decision. There is a lazy consensus mechanism: SC members will have 15 days to vote on open issues.
* **Voting Mechanism:** Votes are cast using "thumbs up" (👍) or "thumbs down" (👎) emojis on the specific GitHub issue or Enhancement Proposal, or via explicit "+1" / "-1" comments.
* **Identity:** Every vote must be associated with the GitHub identity of an active SC member.
* **Resolution:** An issue is considered approved if it reaches the required threshold (majority for standard issues, unanimous for new SC members) at the end of the 15-day lazy consensus period, provided the 33% quorum is met.

## 4. Contributor Lifecycle, Maintainers, & Sub-teams

To scale effectively across multiple repositories, Policy Labs recognizes
different levels of involvement:

* **Users & Contributors:** Anyone who submits an issue, pull request, or participates in discussions.
* **Repo-level Maintainers:** Contributors who have demonstrated consistent merit, technical expertise, and alignment with the project's goals on a specific repository may be granted maintainer status for that repository.

### Promotion Process

Existing maintainers or SC members can nominate a contributor. The SC will vote
on the nomination using the standard emoji voting process. A majority vote
approves the new maintainer.

### Cross-Repo Sub-teams

As the organization grows, the SC may charter sub-teams to govern specific
operational or technical domains across multiple repositories (e.g., a
centralized CI/CD Team, a Documentation Team, or a Security Team). Sub-teams
operate with delegated authority from the SC for their specific domains.

## 5. Intellectual Property & Developer Certificate of Origin (DCO)

To ensure clear intellectual property provenance and comply with Linux Foundation best practices, all contributions to Policy Labs repositories must be accompanied by a Developer Certificate of Origin (DCO).

* All commits must include a `Signed-off-by` line indicating that the contributor agrees to the DCO (version 1.1 or later).
* Pull requests lacking this sign-off will not be merged until the contributor amends their commits to include the proper DCO sign-off.

## 6. Code of Conduct

The Policy Labs organization is committed to providing a welcoming and inspiring community for all.

* All contributors, maintainers, and SC members are expected to adhere to the OpenSSF's [Code of Conduct](https://openssf.org/community/code-of-conduct/).
* Violations of the Code of Conduct will be reviewed and addressed by the Steering Committee, which reserves the right to remove contributors or maintainers who violate these terms.

## 7. End-of-Life (EOL) & Archival Policy

As an organization managing multiple repositories, it is expected that some projects or experiments will naturally reach the end of their useful lifecycle. To keep the organization healthy and clear for users, the following archival process applies:

### Criteria for Archival

A repository may be considered for EOL/Archival if it has been superseded by a
new technology, is no longer aligned with the Policy Labs mission, or has lacked
active maintainers or commits for a period of 6 months or more.

#### Archival Process

1. An SC member or repo maintainer opens an issue proposing the archival of the repository.
2. The SC conducts a standard emoji vote (15-day lazy consensus).
3. If approved, a deprecation notice is added to the top of the repository's `README.md`, directing users to alternatives if applicable.
4. The GitHub repository is officially archived (set to read-only) to preserve its history and code for the public, while clearly indicating it is no longer actively maintained.
