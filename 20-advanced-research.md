# Advanced Research Notes

Recent work increasingly treats prompt injection as an **agent/system problem**, not merely a bad-input problem.

Important themes to watch:

```text
adaptive attacks
concealed side effects
memory poisoning
cross-agent trust
browser-agent attacks
multimodal injection
tool-output injection
system-level defenses
input/tool-output firewalls
provenance-aware context handling
```

A 2025 study of indirect prompt injection defenses found that tool-interface filtering can improve security/utility, but also noted that stronger adaptive attacks can bypass existing benchmark defenses. citeturn634539academia66

A 2026 large-scale red-team competition tested tool-calling, coding, and computer-use agents with hundreds of thousands of attack attempts and found successful attacks across all tested model families, reinforcing the need to test behavior at the system level rather than assuming a single model's refusal behavior is sufficient. citeturn499576academia67

---
