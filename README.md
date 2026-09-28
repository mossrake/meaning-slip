# Meaning Slip

**A framework for AI conversation governance, and the interface for the tracker that measures it.**

Agentic systems run on conversation: models brief other models, agents delegate to agents, and every summary an agent writes is read later, sometimes by itself. Each exchange carries the oldest risk in commerce: the parties can proceed without meaning the same thing. *Meaning slip* is the displacement between two parties' understandings of the same exchange. It is not a property of any message or any endpoint, so per-message checks and endpoint monitoring cannot see it. It is a property of the pair, and it accumulates in what each party separately holds.

The tracker is an observer that sits beside a deployment's inference proxy, never on the call path. It links the exchanges between agents, asks each party from a copy what it understood, compares the two accounts against a calibrated band, and keeps an append-only record. It produces no verdicts and makes no inference about intent.

## What's here

| File | What it is |
| --- | --- |
| [meaning-slip-framework.pdf](meaning-slip-framework.pdf) | The framework paper (July 2026, rev. August 2026). Defines meaning slip, the seven signatures, the four coverage questions, and the measurement program. |
| [semantic-observer-interface-statement.pdf](semantic-observer-interface-statement.pdf) | What the observer needs from an agent runtime: what it must see, what it must be able to do, what it emits, and what it refuses to claim. Written with NVIDIA OpenShell as the worked case; see [OpenShell issue #1272](https://github.com/NVIDIA/OpenShell/issues/1272). |

The observer's design specification (exchange linking, calibration, reader qualification, the propensity battery) is available under a mutual NDA. Contact us through [mossrake.ai](https://mossrake.ai).

## Related

- [Language Model Diligence](https://github.com/mossrake/language-model-diligence): the framework this paper extends from single models to the conversations between them.

---

Mossrake Group, LLC · [mossrake.ai](https://mossrake.ai)
Scott Weller

© 2026 Mossrake Group, LLC. All rights reserved. Mossrake®, Language Model Diligence™ and Language Model Tectonics™ are trademarks of Mossrake Group, LLC.
