# Jake · burrejak22

I write small tools. Security CLIs, browser extensions, Roblox stuff. Node or PowerShell, usually whatever's bugging me that week.

## Lately

**[chess-coach](https://github.com/burrejak22/chess-coach)**
Chrome extension that watches a Lichess or Chess.com board and tells you what a decent player at your rating would actually play, in plain English, with reasons. Purple arrows mark the tempting-looking inaccuracies, gold marks brilliant finds. Runs Stockfish across a Web Worker pool so a few probes chew through the position in parallel.

**[roblox-booster](https://github.com/burrejak22/roblox-booster)**
PowerShell helper that makes Roblox smoother on Windows without touching the Roblox process. Priority bump, GPU preference, a FastFlag preset, and an opt-in FPS unlocker that warns you before Hyperion crashes it. The README doubles as a writeup of every historical Roblox booster trick and why most of them died after anti-cheat landed.

**[showdex](https://github.com/burrejak22/showdex)**
Fork of doshidak's Pokemon Showdown damage-calc extension with a Battle Advisor layer. AGPL-3.0.

## Security CLIs

Four tools. Each answers one question:

- **[crxray](https://github.com/burrejak22/crxray)**: is this Chrome extension safe to allowlist?
- **[pkgvet](https://github.com/burrejak22/pkgvet)**: should I actually `npm install` this?
- **[ciguard](https://github.com/burrejak22/ciguard)**: is this GitHub Actions workflow about to leak a secret?
- **[dangler](https://github.com/burrejak22/dangler)**: do I own any subdomains someone else is about to take over?

Zero-dep Node mostly. All exit non-zero on findings. All take `--json`.

## CTF

**[cryptsmith](https://github.com/burrejak22/cryptsmith)** does the crypto. Classical ciphers, XOR break via hamming-distance keysize guessing, Wiener and Hastad and common-modulus RSA, pcap carving, hash ID. Python stdlib only. **[flaghunter](https://github.com/burrejak22/flaghunter)** sits on top and throws the whole kit at a challenge file or capture, then writes up what fell out.
