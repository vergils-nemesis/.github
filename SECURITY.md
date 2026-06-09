# Security Policy

## Reporting a Vulnerability

If you discover a security vulnerability in this repository, please
report it through
[GitHub's private vulnerability reporting](https://github.com/vergils-nemesis/.github/security/advisories/new).
This ensures your report is handled confidentially.

If private vulnerability reporting is unavailable, email
**w.phillip.moore@gmail.com** with the subject line
"vergils-nemesis Security Report". Do not open a public issue for
security vulnerabilities.

## Scope

`vergils-nemesis` is a documentation-only organization. The single
repository it contains — `.github` — holds the org profile and
community health files. Security reports in scope are limited to
issues in this repository's own configuration that could expose
contributors or the organization, such as a misconfigured workflow or
hook.

The VERGIL tooling itself is developed and reported separately in the
[vergil-project](https://github.com/vergil-project) organization; see
its
[security policy](https://github.com/vergil-project/.github/security/policy).

## Out of Scope

- Vulnerabilities in upstream dependencies (report these to the
  upstream maintainer)
- Vulnerabilities in GitHub, Docker, or other third-party platforms
- Social engineering attacks against project contributors

## Response Commitment

- **Acknowledgment**: within 7 days of receiving a report
- **Assessment**: initial severity assessment within 14 days
- **Resolution**: target fix or mitigation plan within 30 days of
  acknowledgment, depending on severity and complexity

These timelines reflect the project's current scale as a small
community project. Response times may vary, but every report will be
acknowledged and investigated.

## Disclosure Policy

We follow coordinated disclosure. Once a fix is available, we will:

1. Release the fix
2. Publish a security advisory on GitHub
3. Credit the reporter (unless they request anonymity)

We ask that reporters allow reasonable time for a fix before public
disclosure.
