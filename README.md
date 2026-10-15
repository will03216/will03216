<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=26&duration=3200&pause=900&color=58A6FF&center=true&vCenter=true&width=760&lines=Hi%2C+I'm+Will+Zhang+%F0%9F%91%8B;Forward+Deployed+%C2%B7+Solutions+%C2%B7+Software+Engineer;I+turn+customer+problems+into+shipped+AI+systems;MEng+EIE+%40+Imperial+College+London+'27" alt="Typing SVG" />

<p>
  <a href="mailto:zhangjunkaiwill@gmail.com"><img src="https://img.shields.io/badge/Email-zhangjunkaiwill%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Based_in-London%2C_UK-0A66C2?style=flat-square&logo=googlemaps&logoColor=white" />
  <img src="https://img.shields.io/badge/Open_to-FDE_%C2%B7_Solutions_Architect_%C2%B7_SWE_(2027)-2EA44F?style=flat-square" />
</p>

</div>

---

```python
class WillZhang:
    role      = ["Forward Deployed Engineer", "Solutions Architect", "Software Engineer"]
    education = "MEng Electronic & Information Engineering @ Imperial College London (2027)"
    shipped   = {"BytePlus": "Solution Architect Intern — AI agents, MCP, GenAI video",
                 "ByteDance": "iOS Software Engineer Intern — Swift / Objective-C"}
    stack     = ["Python", "TypeScript", "C++", "Swift", "SystemVerilog"]
    languages = ["English", "Mandarin"]
```

I work best **between the customer and the code**. At BytePlus I sat with sales teams and customers, found where their workflow broke, and shipped the fix — a lead-qualification engine, internal agents, an MCP server and a full video studio. Before that I shipped production iOS features at ByteDance. My roots are in systems: I've built a C compiler and a pipelined RISC-V CPU, so I'm comfortable going all the way down the stack when a problem needs it.

---

## 💼 Experience

**Solution Architect Intern · BytePlus (ByteDance), London** <sub>Mar – Sep 2026</sub>
- Built a **lead-generation engine** that replaced manual lead qualification: intent signals → LLM scoring → a multi-agent system where specialist agents compete for the send budget. Knowledge-base-linked outreach lifted the **reply rate by 16%**.
- Worked directly with customers on generated-video defects (identity drift, grid artefacts), traced them to diffusion-model behaviour and fixed them through prompt, framing and resolution changes.
- Shipped a **Seedance MCP server** (SDK + server + CLI + agent skills) so non-engineers could generate video from their AI assistant, deployed once in Docker with server-side credentials.
- Shipped three internal agents for Sales / AE teams: a RAG knowledge-base agent, a pre-call prospecting agent and a Slack daily digest.
- Built **Lumen Hub**, an infinite-canvas AI video studio in Next.js / React.

**iOS Software Engineer Intern · ByteDance, Beijing** <sub>Jul – Oct 2025</sub>
- Built comment-input pre-creation and reuse infrastructure (object pooling, prewarm scheduling): **−20–27 ms first render**, **+0.2–0.48% comment clicks per user**.
- Added a Swift / Objective-C pre-commit quality pipeline (SwiftLint, OCLint, Git hooks) and migrated 4 UI components from Objective-C to Swift.

---

## 🧠 Featured Projects — AI Agents & Customer-Facing Systems

<table>
<tr>
<td width="50%" valign="top">

### [Lead Qualification Engine](https://github.com/will03216/Byteplus_work_cortex)
A "Claude brain" for outbound sales — turns noisy lead exports into a **ranked, auditable** lead list.

- Two-stage LLM pipeline: **evidence extraction → scoring**, separating observed facts from inference
- Python control plane: score clamping, threshold routing, hard disqualifiers
- Per-lead JSON audit artifacts · FastAPI UI · Postgres · Docker
- Provider-agnostic (Claude / Seed 2.0 via `.env`)

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" /> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" /> <img src="https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white" />

</td>
<td width="50%" valign="top">

### [Lumen Hub — AI Video Studio](https://github.com/will03216/lumen-hub)
A self-hostable infinite-canvas studio for **Seedream / Seedance** generation.

- An LLM splits one concept into shots under the model's length limit; **ffmpeg** stitches them server-side into one long video, and interrupted runs resume where they stopped
- *Video Style Extract*: reference clip → style brief → enhanced prompt
- Strict BYOK: per-user **encrypted API keys**, Clerk auth, Postgres
- Dockerised standalone Next.js build with health checks

<img src="https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=nextdotjs&logoColor=white" /> <img src="https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black" /> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" /> <img src="https://img.shields.io/badge/ffmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [Pre-Meeting Customer Profile Agent](https://github.com/will03216/pre-meeting-customer-profile-agent)
Writes account briefings for AEs straight from **Lark calendar events**, domains or emails.

- Scans calendar windows, skips internal meetings, auto-detects the customer's vertical
- Apollo.io + web enrichment with **domain-identity guards** against false matches
- Evidence-labelled answers: *Known / Likely / To Validate / Not Found*
- Industry playbooks · keeps working when optional permissions are missing · packaged as a portable skill

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/Lark_CLI-00D6B9?style=flat-square" /> <img src="https://img.shields.io/badge/Apollo.io-6C47FF?style=flat-square" />

</td>
<td width="50%" valign="top">

### [Slack Daily Digest](https://github.com/will03216/slack_daily_digest_final_cc)
An agent skill (Claude Code / Codex / Mira) that turns Slack into a twice-daily **AI intelligence digest** in Lark Docs.

- Executive summary, TODOs, pipeline, risk signals, per-channel transcripts
- **Self-healing watchdog**: validates output, retries with backoff, escalates
- Local scheduler (launchd / systemd) that catches up on runs missed while the machine was off

<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/Slack_API-4A154B?style=flat-square&logo=slack&logoColor=white" /> <img src="https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white" />

</td>
</tr>
</table>

## 🔌 MCP Servers & SDKs

| Project | What it is | Highlights |
|---|---|---|
| **[Seedance MCP](https://github.com/will03216/Seedance_mcp_final)** | Video generation for Claude Desktop, Cursor, Windsurf & the terminal | SDK + MCP server + CLI + Claude Code skill · submit-then-poll jobs with cancel & history · automatic asset upload for portrait references · edit/extend · checks requests are valid before submitting |
| **[Seedream MCP](https://github.com/will03216/Seedream_mcp_final)** | Image generation across Seedream 4.5 / 5.0 Lite / 5.0 Pro | Zero-dependency SDK · layer decomposition into RGBA cutouts · TOS upload with HMAC signing · CI on Py 3.10–3.12 |

## ⚙️ Systems & Hardware

| Project | What it is | Stack |
|---|---|---|
| **[C → RISC-V Compiler](https://github.com/will03216/Will_Z-compiler)** | Compiles C with pointers, scoped variables, control flow and function calls to RISC-V assembly. Saves live registers to the stack across calls so nested expressions don't overwrite each other | C++ · Flex/Bison · RISC-V |
| **[Pipelined RISC-V CPU](https://github.com/Wazab-75/RISC-V-Team4)** | RV32I, 5-stage pipeline, hazard unit, 2-way set-associative cache — team of 4 | SystemVerilog · Verilator · FPGA |
| **[FPGA Bop It](https://github.com/will03216/Bop_it_FPGA_Game)** | Multiplayer game on DE10-Lite + NIOS II with an AWS game server · [demo](https://youtu.be/o3yO4nKiVIQ) | Verilog · C · Python · AWS |
| **[Self-Balancing Robot](https://github.com/will03216/WhatdoUmean-Electronics_Design_Project_2_Balance_Robot)** | Two-wheeled robot with PID control on ESP32 + MPU6050, Raspberry Pi link | C++ · Python · Embedded |

---

## 🛠 Tech Stack

<p>
  <img src="https://skillicons.dev/icons?i=python,ts,js,cpp,c,swift&theme=dark" /><br/>
  <img src="https://skillicons.dev/icons?i=nextjs,react,fastapi,postgres,docker,linux&theme=dark" /><br/>
  <img src="https://skillicons.dev/icons?i=git,githubactions,aws,verilog&theme=dark" />
</p>

**Agentic AI & LLM:** multi-agent systems · MCP · agent skills · RAG / embedding retrieval · prompt engineering · CrewAI · AgentOps · OpenAI API (GPT, Whisper) · Claude API · video / image / 3D generation APIs<br/>
**Engineering:** Python · TypeScript · C++ · C · SQL · Swift · Objective-C · Bash · SystemVerilog · WebSockets · OAuth · ffmpeg

<div align="center">
<sub>⭐ The repos above are the best place to start. Happy to walk you through any of them.</sub>
</div>
