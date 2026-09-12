# Security policy

This policy applies to every repository in the PHES-ODM organization. It is the
default for repositories that do not publish one of their own.

## Reporting a vulnerability

**Do not open a public issue, and do not post it on Discourse.** A public report
is disclosure before a fix exists.

Use GitHub's private vulnerability reporting. Open the affected repository's
**Security** tab, then **Report a vulnerability**. It is enabled on every public
PHES-ODM repository. Only maintainers see the report, it stays private until
there is a fix, and you do not need anyone's email address.

If you are unsure which repository is affected, report it against
[PHES-ODM](https://github.com/PHES-ODM/PHES-ODM/security) and we will move it.

## Where a vulnerability is plausible

Most PHES-ODM repositories hold documents: the data dictionary, documentation,
mapping files, manuscripts. A vulnerability in a CSV of part definitions is
unlikely.

The code is where real risk sits.

| Repository | Why it matters |
|---|---|
| [PHES-ODM-Validation](https://github.com/PHES-ODM/PHES-ODM-Validation/security) | A package that parses data files supplied by the user |
| [PHES-ODM-Validation-Web](https://github.com/PHES-ODM/PHES-ODM-Validation-Web/security) | A hosted service that accepts uploads |
| [PHES-ODM-Search-MCP](https://github.com/PHES-ODM/PHES-ODM-Search-MCP/security) | A hosted service reachable over the network |
| [PHES-ODM-LinkMLGenerator](https://github.com/PHES-ODM/PHES-ODM-LinkMLGenerator/security) | Generates schemas from the dictionary |
| [PHES-ODM-MapGenerator](https://github.com/PHES-ODM/PHES-ODM-MapGenerator/security) | Generates mapping files |
| [PHES-ODM-Mapper](https://github.com/PHES-ODM/PHES-ODM-Mapper/security) | Reads and transforms source data |

This describes where a vulnerability is likely, not where a report is welcome.
Report anything you find in any repository.

## Testing

Please do not run automated scanning, fuzzing or load testing against the hosted
services. They run on modest hardware and a scan is indistinguishable from an
attack at the receiving end. If you need to test something against a live
service, ask first through a private report and we will arrange it.

Testing against your own local copy needs no permission.

## What happens next

We will acknowledge the report and tell you whether we can reproduce it.

The project is in a
[maintenance phase](https://odm.discourse.group/t/shifting-phes-odm-activity-levels/220)
with limited person-hours, and general responsiveness is slower than it was.
Security reports are the exception and are looked at ahead of other work.

If a fix is needed we will agree a disclosure date with you. If we conclude the
report is not a vulnerability we will say so and explain why, rather than
letting it go quiet.

## Supported versions

Fixes land on the current release. The ODM data model is versioned separately
from the tools, and older model versions are not patched: the current major
version is the supported one. Where a fix affects data already published under
an older version, we will say so in the advisory.

## Credit

We will credit you in the advisory unless you would rather we did not. Tell us
which you prefer when you report.
