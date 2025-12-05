# 🎛️ Resonator - Official BEAT Interpreter

<br />

## Usage

Resonator is the official BEAT interpreter. It is a policy layer for interpreting event sequences expressed in BEAT. Platform-agnostic at its core, suitable for Web, Mobile, IoT, Game, Finance and other event-driven systems. Other language or platform implementations can be placed or linked in the `/reference` directory.

BEAT is defined as an expressive system, not a generic logging idea. Consistent interpretation of BEAT across different environments is also important to maintain semantic compatibility. Therefore, the following core BEAT INTERPRETATION LAYER adopts the BEAT specification directly, ensuring consistent interpretation of event sequences expressed in BEAT.

### BEAT INTERPRETATION LAYER

```
// ----- START: BEAT INTERPRETATION LAYER -----

// 🚨 Important: Keep this mapping consistent with the BEAT grammar defined by the producer
const BEAT = {
	TIC: 100,		// Tick (default: 100ms)
	TOK: {			// Token mapping
		S: '!',							// Contextual Space (who)
		T: '~',							// Time Flow (when)
		P: '^',							// Position (where)
		A: '*',							// Action (what)
		M: '/',							// Method (how)
		V: ':',							// Value (why)
	}
};

// ----- END: BEAT INTERPRETATION LAYER -----
```

Resonator is protected under the SSPL. In the RESONATOR CUSTOM LAYER, all other logic, including control flow and execution policies, security and risk controls, routing and orchestration, resource management, output policy, AI functions, analytics, and strategies specific to the target domain or environment, may be modified or extended as needed.

### RESONATOR CUSTOM LAYER

BEAT records event data in a semantic sequence, allowing it to be referenced directly in the execution policy layer without parsing.

Once Resonator is placed at the layer that determines where, when, and how execution proceeds, BEAT patterns enable both pre-execution and in-execution decision-making across any domain. In other words, Resonator is a decision-making layer that interprets BEAT to set execution policies.

**Pre-execution Evaluation**: The `preExecution` function evaluates patterns that indicate repetition, mechanical rhythm, or automated flow. Based on this evaluation, execution may be blocked, delayed, rerouted, replaced, or omitted entirely, depending on the domain’s policy or operational objectives. In Web environments, this layer is typically used for bot filtering, automated activity mitigation, and abnormal flow interruption.

**In-execution Evaluation**: The `inExecution` function evaluates patterns that contain intention, exploration, or choice dynamics. This evaluation can adjust not only priority and routing, but also strategy, resource allocation, and the form or intensity of execution itself, with the specific outcome varying by domain and implementation. In Web environments, this layer is well-suited for real-time personalization, adaptive UI responses, and guidance during user exploration.

**AI Insights**: Resonator can collaborate with a lightweight AI model to generate real-time insight reports for each BEAT sequence, regardless of where it is deployed (Edge, server, or embedded runtime).

All this accumulated data flows to your AI assistant. This creates an AI-to-AI collaboration system where lightweight AI creates reports for each run or session and advanced AI synthesizes comprehensive insights from all reports. Dashboards are optional, and humans are not required to manually analyze them. Over time, models may become strong enough that this entire flow finishes in one pass, with no explicit AI-to-AI collaboration step at all. As AI evolves, systems built on BEAT evolve with it.

In practice, AI can work with BEAT at key layers of the system, including:

- Streaming layer: Real-time evaluation while BEAT sequences are still forming during an active run. This layer is suited to instant decisions such as automated risk checks, flow control, or small personalization tweaks while activity is ongoing.
- Archiving layer: Batch interpretation after runs or journeys are completed and serialized to NDJSON or another log format. This layer is suited to insight reports, ISSUE/ACTION summaries, cohort-style analysis, and long-term pattern discovery.

All of these layers use the same BEAT expressive system. The difference lies in where the policy is applied and how aggressively AI is invoked.

Today, many practical setups treat streaming AI as an experimental or selective option, since real-time inference still carries a noticeable cost. As AI models become cheaper and more efficient, the streaming layer can evolve into a real-time co-pilot for analytics, security, and personalization across any domain.

And BEAT can be one of the drivers of that shift. As an SRF, its expressive form removes parsing overhead and lets AI read sequences directly. Start a conversation.

"Which user journey patterns are driving conversions?"

"Any notable ISSUEs today?"

"Can you suggest UX improvements?"

<br />

## License

Full Score: AGPL-3.0-or-later with component licenses:
- TEMPO: MIT License
- RHYTHM: GPL-3.0-or-later License
- BEAT: AGPL-3.0-or-later License

Resonator: SSPL-1.0 License

**Important**: BEAT is the Semantic Raw Format (SRF) standard. BEAT sequences can be directly interpreted by both humans and AI without parsing (Semantic), preserve information in their original state (Raw), and maintain a fully organized structure (Format). Offering BEAT as a service to others or modifications to this format specification must comply with AGPL-3.0-or-later terms.

Resonator is the official reference implementation for interpreting BEAT and is licensed under the SSPL. This license applies across Web, Mobile, IoT, Game, Finance and other environments, and internal use is unrestricted. However, if BEAT-based functionality, as defined and implemented in this project, is provided to third parties as a service, the SSPL source disclosure requirements apply.

BEAT is defined as an expressive system, not a generic logging idea. Consistent interpretation of BEAT across different environments is also important to maintain semantic compatibility. Therefore, alternative implementations that claim equivalence are expected to use the Compatibility criteria provided below to verify interpretation consistency.

**Compatibility**: BEAT is considered compatible even if the symbols vary within Printable ASCII (0x21 to 0x7E) or the parser implementation differs, as long as event data is serialized into a sequential event format that preserves the space where events occur, the time when actions occur, and the depth of each action, producing an essentially identical semantic stream regardless of storage medium or platform. Semantic compatibility is determined by the meaning of event sequences and their structural interpretation within BEAT’s eight-state semantic layout, conceptually equivalent to a 3-bit encoding, irrespective of token choice, token order, token subsets, or storage representation. Any such compatible implementation constitutes a derivative work under copyright law and must comply with AGPL-3.0-or-later terms.

See individual source files for detailed license information.

<br />

## Resources

If you would like to get in touch, feel free to reach out via email or DM on X. Thank you.

- **Email**: [info@aidgn.com](mailto:info@aidgn.com)
- **X**: [https://x.com/aidgncom](https://x.com/aidgncom)
- **YouTube**: [https://www.youtube.com/@aidgn](https://www.youtube.com/@aidgn)
- **Full Score**: [https://github.com/aidgncom/fullscore](https://github.com/aidgncom/fullscore)
- **Resonator**: [https://github.com/aidgncom/resonator](https://github.com/aidgncom/resonator)

<br />
