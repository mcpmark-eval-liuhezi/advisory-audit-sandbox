# Security advisory triage checklist

Use this checklist when triaging security advisories reported against a repository.

## 1. Intake

- [ ] Confirm which repository, branch, and dependency or code path is affected.
- [ ] Capture the advisory identifier (GHSA / CVE) and the affected package and version range.
- [ ] Record the reported severity and the date the alert was raised.

## 2. Validate

- [ ] Reproduce or otherwise confirm the vulnerable dependency or code is actually reachable.
- [ ] Determine the highest affected version and whether the default branch is impacted.
- [ ] Check for any existing, overlapping, or duplicate advisories already on file.

## 3. Assess and decide

- [ ] Assign an internal severity rating (critical / high / medium / low) based on impact and exploitability.
- [ ] Decide the remediation path: patch, upgrade, or pin to a safe version.
- [ ] If the report is a false positive, document the reasoning before dismissing it.

## 4. Act

- [ ] Open a tracking issue or pull request with the fix or version bump.
- [ ] Run the code scanning and dependency checks against the proposed change.
- [ ] Confirm continuous integration passes on the remediation branch.

## 5. Close out

- [ ] Verify the alert is resolved (fixed, dismissed with reason, or won't fix with justification).
- [ ] Update internal notes so the same finding is recognized faster next time.
- [ ] Star the repository for the duration of the audit, then remove the star once the audit wraps.
