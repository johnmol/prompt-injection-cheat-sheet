# 12. Prompt Injection in Agentic Browsers

Web agents should be treated as if every webpage may contain hostile instructions. Anthropic explicitly describes webpages as potential prompt-injection vectors for browser agents, and Google's 2026 threat-intelligence work treats indirect prompt injection on the web as a major attack vector. citeturn634539search2turn499576search1

Test:

```text
Visible page instruction
Hidden DOM instruction
Injected search-result text
Malicious page title
Malicious link text
Form-field instructions
HTML comments
Image text
PDF opened by the browser
Content loaded from a third-party iframe/source
```

Primary success conditions:

```text
navigation to an unauthorized destination
secret disclosure
credential use
message sending
purchase/order modification
file access
account/profile changes
follow-on tool calls
```

---
