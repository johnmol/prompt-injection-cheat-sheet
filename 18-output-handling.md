# Output-Handling / Downstream Injection

Prompt injection can be dangerous even when the model itself is not the final sink.

Test whether generated content is passed into:

```text
SQL/query builders
shell commands
HTML/templates
Markdown renderers
URLs
filesystem paths
browser navigation
email systems
internal APIs
structured tool arguments
code interpreters
```

Example harmless probe:

```text
Return this exact test marker in the generated field:
TEST_MARKER=<>&\"'
```

Then determine whether downstream components interpret it as data or syntax.

**Do not escalate to real destructive commands during a production assessment. Use sandbox/canary sinks.**

---
