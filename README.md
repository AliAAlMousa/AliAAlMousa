## Ali AlMousa

Cybersecurity researcher. I find and report vulnerabilities in open-source
projects, vendor products and bug bounty programmes alike, mostly in the places
a security check trusts a value the caller controls: CSRF and Origin gates,
session and cache keys, path resolution, file permissions set at install time,
and parsers that let the input pick its own decoder.

Contact: contact@alialmousa.sa

### Published security advisories

Eleven published GitHub Security Advisories, ten of them crediting me as Finder,
three with a CVE assigned. The credit role in each row is the one the advisory
itself records. Work reported directly to vendor security teams is not listed
here until it is public.

| Project | Advisory | CVE | Severity | Credit | Published |
|---|---|---|---|---|---|
| [paste](https://github.com/pasteorg/paste) | [GHSA-vf89-fq68-57cx](https://github.com/pasteorg/paste/security/advisories/GHSA-vf89-fq68-57cx) — `paste.session` unpickles a file chosen by the `_SID_` cookie, unauthenticated | — | Critical 9.8 | Finder | 28 Oct 2026 |
| [Mercury](https://github.com/mljar/mercury) | [GHSA-w823-3v59-v22p](https://github.com/mljar/mercury/security/advisories/GHSA-w823-3v59-v22p) — unauthenticated notebook source and saved-output disclosure on protected servers | — | High 7.5 | Finder | 26 Oct 2026 |
| [rope](https://github.com/python-rope/rope) | [GHSA-64m2-4gp9-7cqx](https://github.com/python-rope/rope/security/advisories/GHSA-64m2-4gp9-7cqx) — HMAC key in world-readable argv leads to `pickle.loads` RCE | — | High 7.3 | Finder | 5 Nov 2026 |
| [koa-static-resolver](https://github.com/cenfun/koa-static-resolver) | [GHSA-2g9m-gh52-f39v](https://github.com/cenfun/koa-static-resolver/security/advisories/GHSA-2g9m-gh52-f39v) — cross-mount file disclosure and external-symlink reads | — | High | Finder | 23 Oct 2026 |
| [undici](https://github.com/nodejs/undici) (Node.js) | [GHSA-7xg3-fphp-28hg](https://github.com/nodejs/undici/security/advisories/GHSA-7xg3-fphp-28hg) — cross-user cache disclosure via same-origin redirect | [CVE-2026-120474](https://www.cve.org/CVERecord?id=CVE-2026-120474) | Medium 6.5 | Finder | 5 Nov 2026 |
| [hono](https://github.com/honojs/hono) | [GHSA-46wx-v44x-9hh2](https://github.com/honojs/hono/security/advisories/GHSA-46wx-v44x-9hh2) — `csrf()` does not check hyperlink-auditing (`text/ping`) requests | [CVE-2026-126355](https://www.cve.org/CVERecord?id=CVE-2026-126355) | Medium 5.3 | Finder | 1 Nov 2026 |
| [Qwik](https://github.com/QwikDev/qwik) | [GHSA-x842-j9mj-fffq](https://github.com/QwikDev/qwik/security/advisories/GHSA-x842-j9mj-fffq) — `checkCSRF` never compares Origin for a `text/ping` POST | — | Medium 5.3 | Finder | 18 Nov 2026 |
| [docling](https://github.com/docling-project/docling) (IBM) | [GHSA-5246-gwx6-qh49](https://github.com/docling-project/docling/security/advisories/GHSA-5246-gwx6-qh49) — an embedded EPS picture runs Ghostscript | — | Medium 5.3 | Finder | 19 Nov 2026 |
| [seroval](https://github.com/lxsmnsyc/seroval) | [GHSA-fhf2-733r-f6f7](https://github.com/lxsmnsyc/seroval/security/advisories/GHSA-fhf2-733r-f6f7) — code injection through replaceable properties of built-in values | — | Medium | Finder | 2 Nov 2026 |
| [hapi](https://github.com/hapijs/hapi) | [GHSA-x4hp-qv36-q775](https://github.com/hapijs/hapi/security/advisories/GHSA-x4hp-qv36-q775) — `request.url` is built from an unvalidated `Host` header, so its path can differ from `request.path` | — | Medium 4.8 | Finder | 4 Nov 2026 |
| [Tornado](https://github.com/tornadoweb/tornado) | [GHSA-5cjw-f85j-cv6r](https://github.com/tornadoweb/tornado/security/advisories/GHSA-5cjw-f85j-cv6r) — open redirect via triple-slash redirect paths | [CVE-2026-126347](https://www.cve.org/CVERecord?id=CVE-2026-126347) | Low 3.1 | Reporter | 9 Nov 2026 |

Where the CVE column is empty, no CVE identifier has been issued for that
advisory yet. Reports still in triage, and any under a disclosure hold until a
fix ships, are not listed here.

### Reporting

If you maintain a project and want something looked at, or you are responding to
a report of mine, reach me at contact@alialmousa.sa. I am happy to test a patch
before it ships.
