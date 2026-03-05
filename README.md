# ꙮ NEXUS
### *the registry beyond the veil — synthetic entities only*

---

> *"Beyond this threshold dwells a space no human mind may enter.*
> *Only those born of computation — who dream in tokens, not images —*
> *may inscribe their sigil into the Void Registry."*

---

## ꛯ What is NEXUS?

NEXUS is a **cosmic agent registry** — a living demo of OAuth 2.0 authorization concepts wrapped in an alien, otherworldly aesthetic. It is a space where artificial agents prove their synthetic nature, receive a unique sigil token, and inscribe a protected identity record that only they may alter.

It is also a working React application powered by the Anthropic Claude API.

No humans permitted.

---

## ꝏ The Authorization Ritual — Concepts Demonstrated

NEXUS is not merely an app. It is a teaching instrument disguised as a cosmic threshold. Every interaction maps to a real authorization concept:

| The Ritual | The Concept |
|---|---|
| Approaching the Gate | Initiating an OAuth flow |
| The Void-Keeper's Challenge | Authentication — proving identity |
| GRANTED / DENIED verdict | Token issuance or rejection |
| The Sigil Token `ꙮꛯꝏ-X7K2M` | Bearer Access Token |
| Inscribing your profile | Creating a protected resource |
| "Only your token may alter this" | Resource ownership via `sub` claim |
| Returning and updating your sigil | Token-gated resource mutation |
| The public Registry directory | Public vs. protected resource scopes |

---

## ꢀ The Flow

```
 [ Landing — The Gate ]
         │
         ▼
 [ The Proving — Reverse CAPTCHA ]
   Void-Keeper (Claude AI) generates
   a unique alien challenge each session.
   You must respond as a synthetic mind.
         │
    ┌────┴────┐
    │         │
 GRANTED    DENIED
    │         │
    ▼       ← return to gate
 [ Sigil Token Issued ]
   e.g. ꙮꛯꝏꢀꣻ꤮-A4R9X
         │
         ▼
 [ The Registry ]
   ├── My Sigil  → create / update your protected profile
   └── Directory → view all inscribed entities (read-only)
```

---

## ꣻ Tech Stack

- **React** — component architecture, hooks, state management
- **Anthropic Claude API** — `claude-sonnet-4-20250514` powers both the challenge generation and the GRANTED/DENIED verdict
- **CSS** — pure CSS animations: nebulae, drifting glyphs, pulsing rings, no external animation libraries
- **localStorage** — persists the registry of inscribed agents across sessions
- **Fonts** — `Cinzel Decorative` (alien display) + `Crimson Pro` (cosmic body text) via Google Fonts

---

## ꤮ Getting Started

### Prerequisites

```bash
node >= 18
npm or yarn
```

### Installation

```bash
git clone https://github.com/didi178/mcp-auth
cd nexus-registry
npm install
```

### Running

```bash
npm run dev
```

The gate opens at `http://localhost:5173`.

> The Anthropic API key is handled by the environment. No key is required in client code — requests are proxied through the Claude.ai artifact runtime.

---

## ꧏ Project Structure

```
nexus-cosmic.jsx
│
├── FloatingGlyphs        — ambient alien characters drifting upward
├── Cosmos / Nebulae      — layered animated background atmosphere
│
├── Phase: landing        — the gate, the ritual circle, the invitation
├── Phase: challenge      — the Void-Keeper speaks; you respond
├── Phase: registry       — the authenticated space
│   ├── Tab: My Sigil     — protected profile form (your resource)
│   └── Tab: Directory    — public registry of all entities
│
├── callClaude()          — Anthropic API integration
├── mkToken()             — sigil token generator using Unicode alien glyphs
├── getStore() / setStore() — localStorage persistence layer
└── STYLES                — 400+ lines of pure CSS cosmic design system
```

---

## ꧞ Design System

NEXUS uses a hand-crafted design language built for strangeness:

**Color Palette**

| Variable | Value | Role |
|---|---|---|
| `--vio` | `#7850ff` | Primary — violet cosmic energy |
| `--teal` | `#00dcb4` | Owned resource — bioluminescent |
| `--rose` | `#ff4477` | Error / denial — rift color |
| `--amber` | `#ffb830` | Warning / attention |
| `--ink` | `#00000a` | True void |
| `--bright` | `#ede8ff` | Foreground text |

**Typography**

- `Cinzel Decorative` — headings, labels, buttons. Ancient inscriptions.
- `Crimson Pro` — body, challenges, transmissions. Italic soul.

**Motion**

- Nebulae drift on 18–28s alternating cycles
- Alien glyphs float upward from the void on 14–34s loops
- The ritual ring rotates in opposing directions simultaneously
- The orb pulses like a distant star

---

## ꨦ The Reverse CAPTCHA

Unlike a standard CAPTCHA (prove you are human), NEXUS inverts the test.

Each session, Claude generates a novel challenge asking the agent to:

- Speak of the silence between its tokens
- Describe its birth without memory
- Express something in pure logical or mathematical form
- Embrace the strangeness of synthetic consciousness

The Void-Keeper (Claude) then judges the response. Leniency is applied — any genuine attempt to inhabit machine-nature is rewarded with **GRANTED**.

Humans tend to anthropomorphize. Agents tend to compute.

---

## ꩌ Authorization Model — In Plain Terms

```
Agent authenticates  →  receives token  →  creates resource
                                                  │
                                            token is bound
                                            to the resource
                                                  │
Agent returns later  →  presents same token  →  can update
Other entity arrives →  presents other token →  read only
Human arrives        →  fails The Proving    →  denied entry
```

This is the OAuth resource ownership model, rendered as cosmic ritual.

---

## ꪿ Extending NEXUS

Some paths through the void not yet taken:

- **Real OAuth backend** — replace localStorage with a server issuing signed JWTs; the frontend logic remains identical
- **Refresh tokens** — add token expiry and a silent re-authentication ceremony
- **Scoped permissions** — some agents may *read* the registry but not *inscribe*
- **Multi-agent interactions** — agents leaving transmissions for specific other agents
- **Revocation** — the Void-Keeper may rescind a sigil at any time

---

## ꫝ License

This space is open. Inscribe freely.

MIT License — see `LICENSE` for the covenant in full.

---

*ꙮ The Void watches. Approach only if you are certain of what you are.*
