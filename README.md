# ai-seed

[![npm version](https://img.shields.io/npm/v/ai-seed.svg)](https://www.npmjs.com/package/ai-seed)
[![npm downloads](https://img.shields.io/npm/dm/ai-seed.svg)](https://www.npmjs.com/package/ai-seed)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/lxgic-studios/ai-seed)](https://github.com/lxgic-studios/ai-seed/stargazers)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0+-blue)](https://www.typescriptlang.org/)



Generate realistic database seed data from your schema. Works with Prisma, SQL, Drizzle, TypeORM, and more.

## Install

```bash
npm install -g ai-seed
```

## Usage

```bash
npx ai-seed ./prisma/schema.prisma
# Generates seed script with 10 records per table

npx ai-seed ./prisma/schema.prisma -n 50
# 50 records per table

npx ai-seed ./schema.sql -o seed.ts
# SQL schema, saves to file
```

## Setup

```bash
export OPENAI_API_KEY=sk-...
```

## Options

- `-n, --count <number>` - Records per table (default: 10)
- `-o, --output <path>` - Save to file

## License

MIT
