# Codewars Katas

JavaScript solutions to Codewars kata challenges, each with Jest unit tests and a Husky pre-commit hook that runs tests before every commit.

## Tech Stack
- JavaScript (ES6+)
- Jest (testing)
- Husky (pre-commit hooks)

## Project Structure
```
codewars-katas/
├── 5-kyu/
├── 6-kyu/
├── 7-kyu/
├── 8-kyu/
│   └── <kata-name>/
│       ├── index.js       # Solution
│       └── index.test.js  # Jest tests
└── package.json
```

## Development
```bash
# Install dependencies
npm install

# Run all tests
npm test

# Scaffold a new kata
npm run create-kata
```

## Key Notes
- Husky pre-commit hook runs `npm run lint && npm run test` automatically; both must pass before a commit is accepted.
