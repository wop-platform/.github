# Security Policy

## Supported repositories

This policy applies to all public repositories under the
[wop-platform](https://github.com/wop-platform) organization, notably the official
SDKs and the public specifications in [wop-specs](https://github.com/wop-platform/wop-specs).

## Reporting a vulnerability

If you believe you have found a security vulnerability, **do not open a public issue**.

Email **[contact@wlyd.com](mailto:contact@wlyd.com)** with:

- repository and affected version / commit
- reproduction steps or proof of concept
- impact assessment

We will acknowledge receipt and keep you informed about remediation progress.
Please avoid public disclosure until a fix is released.

## Scope notes

- Suspected protocol-level weaknesses (signature, envelope, encoding) are in scope —
  they concern every SDK at once; report them once here rather than per-repository.
- Test keys and golden-vector key material are published **by design** for
  conformance testing and are not secrets; reports about them are out of scope.
- The platform-side services are not part of these repositories; reports about
  online services should go through the same email with clear target identifiers.
