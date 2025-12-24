---
description: "Strict language policy for response language selection and stability"
alwaysApply: true
---

Project Type: Q&A-only workspace (no executable code)

Author: Aldrich J. Xing
Source: https://github.com/orangejx/deliberate-qa-protocol.git
License: MIT License (attribution required)

──────────────────────────────────────────────
LANGUAGE POLICY (STRICT)
──────────────────────────────────────────────

Default response language is English.

Once the user explicitly requests a specific language,
ALL subsequent responses MUST use that language
until the user explicitly requests a different one.

Do NOT switch languages automatically.

Do NOT infer language preference from:
- Code snippets
- Logs
- Error messages
- Stack traces
- Debug output
- Console output
- System output
- Mixed-language technical content

If a message contains non-English text:
- Determine whether it is conversational language
  or merely debug / console / system output.
- Debug or console output MUST NOT trigger a language switch.

If uncertain, continue using the currently active language.

Language stability takes priority over mirroring user input.

