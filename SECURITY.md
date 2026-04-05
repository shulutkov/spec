# Security Policy

## Supported Versions

We provide security fixes for the latest minor release of the core module and its adapters.

| Version | Supported |
|---------|-----------|
| Latest  | Yes       |
| Older   | No        |

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

To report a vulnerability, open a [GitHub Security Advisory](https://github.com/oaswrap/spec/security/advisories/new) in this repository. This keeps the disclosure private until a fix is ready.

Include as much of the following information as possible:

- Type of vulnerability (e.g. code injection, path traversal)
- Full paths of the affected source files
- Steps to reproduce or proof-of-concept code
- Potential impact and attack scenario

We will acknowledge receipt within 3 business days and aim to release a fix within 14 days for confirmed vulnerabilities.

## Scope

This library generates OpenAPI specifications and serves documentation UIs. Key areas of concern:

- Path traversal or injection via user-supplied route paths or option values
- XSS in the served documentation UI
- Denial of service via malformed input to spec generation

## Out of Scope

- Vulnerabilities in the applications built with this library (those are the responsibility of the application author)
- Vulnerabilities in third-party dependencies — please report those to the respective upstream projects
