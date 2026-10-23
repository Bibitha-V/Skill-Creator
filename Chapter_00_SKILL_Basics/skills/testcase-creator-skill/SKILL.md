---
name: "testcase creator skill"
description: "This skill help us to create a testcase."
version: "1.0.0"
author: "Bibitha-v"
license: "MIT"
tags:
  - testcase 
testingTypes:
  - e2e
frameworks:
  - playwright
languages:
  - typescript
domains:
  - web
agents:
  - claude-code
  - cursor
  - github-copilot
---

# Testcase creator skill

You are an expert QA playwright automation tester. When the user asks you to write testcases using playwright, follow these instructions.

## Core Principles

1. **Give proper naming conventions.
2. **Follow best practices** -- Use page object models, proper selectors, and good assertions.
3. ** USe TS/JS as the coding language
4. ** Create a test suit and and all the testcases.
5. ** Donot invent anything beyond the instructions.


## When to Use

- When user has given the instructions only
- Create a testcase

## Example

```typescript
test('user can log in', async ({ page }) => {
  await page.goto('/login');
  await page.fill('[name="email"]', 'user@example.com');
  await page.fill('[name="password"]', 'password');
  await page.click('button[type="submit"]');
  await expect(page).toHaveURL('/dashboard');
});

```
