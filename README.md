# Avoid overengineering

A short skill for AI coding assistants that keeps work focused on completing what you asked for.

It favors short working code, reuse of existing code and platform features, and fixes that address the cause across affected callers. It avoids unnecessary features, dependencies, blocking checks and work for hypothetical future needs. Required safeguards and useful tests stay in place. Fewer lines never justify dropping requested behavior.

Use [SKILL.md](avoid-overengineering/SKILL.md) for coding, fixes, reviews and test changes. Copy the `avoid-overengineering` folder into your assistant's skills directory, or provide the file as reusable instructions.
