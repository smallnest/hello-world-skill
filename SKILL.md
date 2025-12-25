---
name: hello-world
description: A simple greeting skill that says hello to the user or a specified name. Use when you need to generate a friendly greeting message or demonstrate basic skill functionality.
license: MIT
metadata:
  author: smallnest
  version: "1.0.0"
---

# Hello World Skill

This is the simplest possible skill that demonstrates the Agent Skills format. It generates a friendly greeting message.

## When to Use This Skill

Use this skill when:
- The user asks for a greeting or to be greeted
- You need to say hello to someone by name
- You want to test or demonstrate basic skill functionality

## How It Works

This skill generates a greeting message in the format "Hello, [name]!" where [name] can be:
- A name provided by the user
- "World" as the default if no name is specified

## Instructions

1. Check if the user has provided a name to greet
2. If no name is provided, use "World" as the default
3. Generate the greeting message: "Hello, [name]!"
4. Optionally include a timestamp of when the greeting was generated

## Examples

### Example 1: Default Greeting

**User request:** "Say hello"

**Output:**
```
Hello, World!
Generated at: 2024-12-25 10:30:00 UTC
```

### Example 2: Personalized Greeting

**User request:** "Say hello to Alice"

**Output:**
```
Hello, Alice!
Generated at: 2024-12-25 10:30:00 UTC
```

### Example 3: Multiple Names

**User request:** "Greet Bob and Charlie"

**Output:**
```
Hello, Bob!
Hello, Charlie!
Generated at: 2024-12-25 10:30:00 UTC
```

## Edge Cases

- **Empty name:** Treat as if no name was provided, use "World"
- **Special characters in name:** Include them in the greeting as-is
- **Very long name:** Accept and use the full name provided

## Output Format

The greeting should be clear and friendly. Include:
1. The greeting message
2. A timestamp (optional but recommended)

Keep the output simple and human-readable.
