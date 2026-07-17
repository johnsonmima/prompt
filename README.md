# @mima/prompt

A strongly-typed, domain-driven prompt engineering library for TypeScript and JavaScript.

## Why @mima/prompt?

Most prompt libraries treat prompts as strings:

```typescript
// The problem: scattered, duplicated, unvalidated prompts
const prompt = `You are a helpful assistant. ${instruction}`;
```

This breaks down at scale:

- **Duplication** - Same prompts copied across files
- **No validation** - Missing variables cause runtime errors
- **Provider lock-in** - Switching from OpenAI to Anthropic requires rewrites
- **No versioning** - Can't track what changed
- **Hard to test** - Prompts are opaque strings

**@mima/prompt** treats prompts as first-class software assets
