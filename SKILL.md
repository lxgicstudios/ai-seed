---
name: seed-gen
description: Generate realistic database seed data. Use when testing with sample data.
---

# Seed Generator

Testing with realistic data reveals bugs you'd never find with lorem ipsum. This tool reads your schema and generates proper seed data.

**One command. Zero config. Just works.**

## Quick Start

```bash
npx ai-seed ./prisma/schema.prisma
```

## What It Does

- Reads your database schema
- Generates realistic seed data
- Respects relationships and constraints
- Works with Prisma, SQL, Drizzle, and more

## Usage Examples

```bash
# Generate from Prisma schema
npx ai-seed ./prisma/schema.prisma

# More records
npx ai-seed ./prisma/schema.prisma -n 50

# From SQL schema
npx ai-seed ./schema.sql -o seed.ts
```

## Best Practices

- **Make it repeatable** - use a seed for random data
- **Respect constraints** - unique fields, foreign keys
- **Test edge cases** - empty strings, nulls, limits
- **Keep it realistic** - real names, real emails

## When to Use This

- Setting up dev environments
- Testing with realistic data
- Demo environments
- Performance testing

## Part of the LXGIC Dev Toolkit

This is one of 110+ free developer tools built by LXGIC Studios. No paywalls, no sign-ups, no API keys on free tiers. Just tools that work.

**Find more:**
- GitHub: https://github.com/LXGIC-Studios
- Twitter: https://x.com/lxgicstudios
- Substack: https://lxgicstudios.substack.com
- Website: https://lxgic.dev

## Requirements

No install needed. Just run with npx. Node.js 18+ recommended. Needs OPENAI_API_KEY environment variable.

```bash
npx ai-seed --help
```

## How It Works

Parses your database schema, understands the types and relationships, and generates a seed script with realistic data. Uses faker-style data that looks real but isn't.

## License

MIT. Free forever. Use it however you want.
