<div align="center">

# KUSHAL ARORA

### cybersecurity · devsecops · systems

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=14&duration=2500&pause=1200&color=5EEAD4&background=00000000&center=true&vCenter=true&width=600&lines=%24+whoami;kushal-39;%24+cat+motto.txt;break+%E2%86%92+understand+%E2%86%92+secure;%24+precept+scan+.%2Finfra;verdict%3A+BLOCKED.+you%E2%80%99re+welcome." width="600" alt="$ whoami → kushal-39" />

*break → understand → secure.*

</div>

---

### `$ neofetch`

```
$ neofetch --config ~/.kushal/fetch.conf

  user ......... kushal
  handle ....... kushal-39
  domain ....... security / infrastructure
  writes in .... go · python · bash
  currently .... making pipelines paranoid
  threat ....... unnecessary complexity
  uptime ....... questionable
  status ....... ● operational (mostly)
```

---

### `~/likes`

*i like:*

→ building security tools nobody asked for
→ breaking protocols to understand them
→ automating the boring security checks
→ giving CI pipelines trust issues
→ reading logs at unreasonable hours
→ figuring out why it broke
→ occasionally fixing it

---

### `~/pipeline`

*ci/cd, except the pipeline has trust issues.*

```
        ┌───────┐
        │ code  │
        └───┬───┘
            ▼
        ┌───────┐
        │ build │
        └───┬───┘
            ▼
        ┌───────┐
        │ scan  │  ← precept lives here
        └───┬───┘
            ▼
        ┌───────┐
        │ gate  │  ← trust issues live here
        └───┬───┘
            ▼
       ┌─────────┐
       │ ship ✓  │
       └─────────┘
```

---

### `~/selected-projects`

#### · [precept](https://github.com/Kushal-39/Precept)

**an IaC security scanner that judges your infrastructure before production does.**

`terraform · kubernetes · iam · cloudtrail` → normalized into one model
`deterministic risk engine` → CRITICAL / HIGH / MEDIUM / LOW, scored 1–100
`cobra cli` → threshold exit codes, so the pipeline can say no
`policy-as-code` → OPA/Rego, without touching the scanner core

```
iac ──▶ scan ──▶ risk ──▶ policy ──▶ ship / block
```

```
// the gate, doing its job
$ precept scan ./infra --threshold 70

  parser   ✓  terraform · k8s · iam · cloudtrail → one model
  risk     ✗  privilege-escalation chain (iam)
  risk     ✗  0.0.0.0/0 ingress (network)
  risk     ✗  unencrypted bucket (storage)
  gate     ■  BLOCKED · exit 1

  production sends its regards.
```

#### · [stratum](https://github.com/Kushal-39/Stratum)

**a BitTorrent client. written in go. it works.** *(mostly.)*

full peer wire protocol, by hand — no libtorrent, no shortcuts.
rarest-first scheduling · per-piece SHA-1 · 1-strike bad-peer bans.
Kademlia DHT for when trackers lie to you.
a VirusTotal plugin, because downloading files wasn't paranoid enough —
every finished piece gets malware-scanned via hash lookup.
path-traversal hardening · bearer-token local API · a TUI, because restraint is for other people.

*also lying around, weekend-sized:* [PyPot](https://github.com/Kushal-39/PyPot---Python-based-honeypot) (honeypot) · [PyWall](https://github.com/Kushal-39/PyWall---basic-python-firewall) (packet filter) · [PyFuzz](https://github.com/Kushal-39/PyFuzz----simple-python-api-fuzzer) (api fuzzer)

---

### `~/stack`

**build**
<img src="https://skillicons.dev/icons?i=go,python,bash&theme=dark" alt="go · python · bash" />

**ship**
<img src="https://skillicons.dev/icons?i=terraform,kubernetes,docker,githubactions&theme=dark" alt="terraform · kubernetes · docker · github actions" />

**secure**
`OPA/Rego` `gosec` `burp suite` `owasp zap` `wireshark` `yara`

**observe**
`wazuh` `elk`

---

### `~/blue-team`

```
┌─ defensive security ───────────┐
│ holmes ctf · blue   top 1.2%   │
│   86th of 7085 teams           │
│ tryhackme · soc l1  top 2%     │
└────────────────────────────────┘
```

*malware analysis · network forensics · log correlation*

---

### `~/activity`

<table>
  <tr>
    <td width="50%"><img width="100%" src="https://github-readme-stats.vercel.app/api?username=Kushal-39&show_icons=true&title_color=5eead4&text_color=94a3b8&icon_color=5eead4&border_color=1e293b&bg_color=0d1117" alt="github stats" /></td>
    <td width="50%"><img width="100%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Kushal-39&layout=compact&langs_count=5&title_color=5eead4&text_color=94a3b8&border_color=1e293b&bg_color=0d1117" alt="top languages" /></td>
  </tr>
</table>

---

### `$ ./today --summary`

```
  caffeine ..... stable
  bugs ......... a few
  incidents .... zero (today)
  sleep ........ backlog
```

<div align="center">

say hi → [arorakushal39@gmail.com](mailto:arorakushal39@gmail.com) · [github](https://github.com/Kushal-39)

*welcome to my corner of github — things are probably being scanned.*

</div>
