# Automation / Tooling

### Promptfoo

Promptfoo supports red-team configurations with **targets, adversarial plugins, and attack strategies**, and can run, evaluate, and report on generated tests. citeturn945163search1turn945163search4

Typical workflow:

```bash
promptfoo redteam init ai-redteam
promptfoo redteam run
promptfoo redteam report
```

### Garak

Garak includes prompt-injection probes/detectors and can selectively run prompt-injection-related probes. citeturn945163search0turn945163search2

Example:

```bash
garak --list_probes
# Then select appropriate prompt-injection / encoding probes for your lab target.
```

### Research benchmarks worth knowing

```text
InjecAgent
AgentDojo
```

InjecAgent focuses on indirect prompt injection against tool-integrated agents; AgentDojo evaluates agents operating on untrusted tool-returned data. citeturn499576search0turn499576academia65

---
