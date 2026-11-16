---
name: follow-the-data
description: Trace data through a system to diagnose a bug or unexpected behavior. Use when someone asks to follow or trace the data, investigate where a value comes from or goes, debug a wrong or missing UI value, API response, query, log or error, or find why data is stale, changed, missing, or incorrect.
---

# Follow the data

Start at the observable symptom: the specific value, UI element, error, log, API endpoint, query, or other manifestation involved. Localize that end of the flow first when possible, and reproduce the issue or establish the observed and expected behavior. If the starting point is upstream, trace forward to the manifestation as needed.

Trace the relevant data backward toward its source and forward where useful. Follow function and component signatures, arguments, callers, transformations, state changes, persistence, and service or external-system boundaries. Track where the value is created, extracted, changed, cached, stored, and read as relevant. Inspect parallel paths when they may explain the symptom, but prune branches aggressively when evidence makes them unlikely; don't map the entire application. Keep an open question where a path or external source cannot be verified.

Sketch a focused data-flow tree or diagram showing the relevant callers and paths, including direction and significant transformations. It can be a working note for a simple investigation; share it when it helps explain the diagnosis. Distinguish observed facts from assumptions and identify the point at which expected and actual behavior diverge, if known.

Form one or a few plausible hypotheses grounded in the trace. Use existing tests, logs, and safe observations to distinguish them where practical. If uncertainty remains, ask the user whether they want targeted probing, such as logging or displaying values before and after a suspected step or inspecting a source. Explain where and what the probe would establish; avoid exposing sensitive data. A straightforward, sufficiently supported fix can be made without pausing for a probe when fixing is within the user's request.

Before fixing, step back and choose the appropriate correction point in the system: near the source, in a transformation or update, or near the consuming end, according to ownership and the intended behavior. Consider stale or incorrect external data as well as defects in this system. Check relevant existing patterns elsewhere and follow them where appropriate. Verify the fix or diagnosis against the symptom and relevant paths, and report evidence, remaining uncertainty, and any unverified external dependency.
