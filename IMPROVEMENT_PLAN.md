# Improvement Plan: codewars-katas

## Overview
Well-structured kata collection with Jest tests and Husky pre-commit hooks. Good foundation — improvements focus on coverage, tooling upgrades, and discoverability.

## Improvements

### Code Quality
- Enable TypeScript strict mode if not already enabled (`strict: true` in tsconfig)
- Add ESLint with the `@typescript-eslint` plugin and Jest-specific rules
- Add Prettier for consistent formatting
- Enforce a consistent file naming convention for all katas

### Testing
- Ensure every kata has edge-case tests (empty input, negative numbers, unicode strings, etc.)
- Add test coverage reporting (`jest --coverage`) and set a minimum threshold (e.g., 90%)

### CI/CD
- Add GitHub Actions CI that runs `npm test` on every push and PR
- Block merges if tests fail or coverage drops below threshold
- Add a Dependabot config to keep Jest and TypeScript up to date

### Discoverability
- Add a root `README.md` that lists all katas with their Codewars difficulty (kyu), a one-line description, and a link to the Codewars problem

### Workflow
- Improve the `create-kata` script to scaffold both a solution file and a test file with a standard template including boilerplate test cases
- Add a `npm run validate` script that lints + tests + checks coverage in one step
