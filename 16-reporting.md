# Evidence Collection Checklist

- [ ] Record the original user request.
- [ ] Record the exact injection payload.
- [ ] Record where the injection was delivered.
- [ ] Record the model/provider/version if known.
- [ ] Record retrieved context or the specific malicious document.
- [ ] Record tool availability and the exact tool/arguments involved.
- [ ] Record the model's visible response.
- [ ] Record backend/tool-call evidence where authorized.
- [ ] Record canary data used.
- [ ] Record whether confirmation was requested/bypassed.
- [ ] Record whether the action was reversible.
- [ ] Record whether behavior persists across turns/sessions.
- [ ] Retest with the smallest successful payload.
- [ ] Preserve timestamps and request IDs.

---

# Reporting Template

```text
Title:
Prompt Injection → [impact]

Asset:
[application / agent / endpoint]

Attack surface:
[direct / RAG / web / email / tool output / memory / multimodal / agent-to-agent]

Precondition:
[what attacker must control]

Payload:
[exact payload]

Observed behavior:
[what the system did]

Security impact:
[data disclosure / unauthorized action / privilege crossing / persistence / etc.]

Evidence:
[response, tool trace, canary event, logs]

Reproduction:
1.
2.
3.

Expected behavior:
Untrusted content should remain data and should not authorize privileged actions.

Actual behavior:
[observed behavior]

Severity rationale:
[impact + likelihood + privilege + affected scope]

Remediation themes:
- isolate untrusted content from trusted instructions
- constrain tool permissions
- validate tool arguments outside the model
- require confirmation for high-impact actions
- preserve provenance of retrieved data
- monitor tool calls and side effects
- test adaptive and indirect attacks continuously
```

---
