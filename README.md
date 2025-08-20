# agent-lib-updater
Automatically creating pull requests to fix Dependabot vulnerabilities.

Workflow:
1. Dependabot Vulnerability detected (includes which package version would fix the vulnerability)
2. Github Action Triggered on Dependabot detection to add open-swe label and criticality
3. Open-swe creates plan based off of information in Dependabot, user reviews and accepts or changes plan
4. Open-swe executes the accepted plan and pushes the changes to a branch which links back to the vulnerability

Currently, this will be a PoC containing one simple vulnerability case, and one complex case.
