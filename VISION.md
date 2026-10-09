# OpenLiate — India's Backend as an Agent Platform

> **Open Source Backend as an Agent (BaaA).**  
> **Class is an Agent. Agent is an API. That's your Backend.**  
> **Backed by the @SarvamAI Startup Program (Bengaluru, India)**

---

### The Evolution: From Hello World to Hello Agent

Software engineering evolves in 50-year paradigm shifts:

- **1972 (Procedural):** `printf("Hello, World\n");`
- **1995 (Object-Oriented):** `class HelloWorld { ... }`
- **2026 (Agent-Oriented):** `class HelloAgent extends LiateAgent { ... }`

**If you know how to write a class, you already know how to build an autonomous AI agent.**

---

### The 5 Foundational Pillars: L - I - A - T - E

OpenLiate is built directly on the **5 Core Architectural Blocks (`Liate_Blocks`)**:

| Pillar | Block Class | What It Manages |
| :---: | :--- | :--- |
| **L** | **`LiateLlm`** | Model provider (Sarvam AI 105B Indic, Gemini Nano, OpenAI) |
| **I** | **`LiateIntegration`** | Memory, Vector Storage, Sessions, Databases & Webhooks |
| **A** | **`LiateAgent`** | The Core Agent Orchestrator, Intent, Skills & Swarms |
| **T** | **`LiateTools`** | Tool Registry, Functions, MCP Protocols & APIs |
| **E** | **`LiateEnv`** | Environment, Guardrails, Timeouts, Spending & Max Turns |

---

### The First Code: Hello AI Agent World

Here is the real, working **Hello Agent** instantiated with the native `L-I-A-T-E` blocks:

```typescript
import { LiateAgent } from "@openliate/liate";

// The Native L-I-A-T-E Class
export class HelloAgent extends LiateAgent {
  constructor() {
    super({
      L: "sarvam/sarvam-105b",            // [L] LiateLlm: Model Provider
      I: { memory: "session-hello" },     // [I] LiateIntegration: Memory & Session
      A: { name: "hello-agent" },         // [A] LiateAgent: Name & Skills
      T: [],                              // [T] LiateTools: Tools & MCPs
      E: { MAX_TURNS: 3 }                 // [E] LiateEnv: Runtime Guardrails
    });
  }
}

// Hello AI Agent World!
const agent = new HelloAgent();
const result = await agent.run("Hello AI Agent World!");
console.log(result.answer);
```

---

### Universal Across All 100M+ OOP Developers

AOP is a universal paradigm for any language that supports a `class`:

* **TypeScript / JavaScript:**  
  `export class HelloAgent extends LiateAgent { ... }`
* **Python:**  
  `class HelloAgent(LiateAgent): ...`
* **Java:**  
  `public class HelloAgent extends LiateAgent { ... }`
* **C# / .NET:**  
  `public class HelloAgent : LiateAgent { ... }`

---

### Core Pillars

1. **Backend as an Agent (BaaA):** The class itself is the standalone runtime and API. Zero external servers required.
2. **Sovereign Indic Intelligence:** Proud member of the **Sarvam AI Startup Program** powering native Indic multilingual agent backends.
3. **100% Free & Open Source (MIT):** Free forever. Self-host it on your own silicon, V8 isolate, or edge runtime with zero vendor lock-in.
4. **Universal Interoperability (BYOA):** Import existing tools and agents from LangChain and CrewAI directly without rewriting code.

---

### The 100-Day Journey (Day 0 ➔ Day 100)

Building in public every single day from Bengaluru, India.  
**10 PM Build. 10 AM Ship.**

- **Website:** [openliate.tech](https://openliate.tech)
- **Repository:** [github.com/openliate/openliate](https://github.com/openliate/openliate)
- **Package:** [npm i @openliate/liate](https://www.npmjs.com/package/@openliate/liate)
- **X / Twitter:** [@OpenLiate](https://x.com/OpenLiate)
