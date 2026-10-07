# Jake · burrejak22

I build small security CLIs for the software supply chain — fast, dependency-light, and CI-friendly.

## The toolkit

**[crxray](https://github.com/burrejak22/crxray)** — X-ray for Chrome extensions. Audits permissions, host access, permission combos, hardcoded secrets, and code for risky patterns. Know what that "productivity" extension is really doing.

**[ciguard](https://github.com/burrejak22/ciguard)** — Security auditor for GitHub Actions workflows. Catches script injection, unpinned actions, `pull_request_target` footguns, secret exfiltration, and cache poisoning.

**[pkgvet](https://github.com/burrejak22/pkgvet)** — Vet an npm package *before* you install it. Install scripts, typosquatting, maintainer count, staleness, repo mismatches. Zero dependencies.

**[dangler](https://github.com/burrejak22/dangler)** — Find dangling DNS records and subdomain takeover risks before attackers do. Certificate-transparency enumeration, 25 service fingerprints, DNS wordlist fallback. Zero dependencies.

All four share one philosophy: **one command, one scored report** — with `--json` and `--fail-on` so they slot straight into CI.

```bash
npx @burrejak/crxray ./my-extension --fail-on HIGH
```
