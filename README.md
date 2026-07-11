<h1 align="center">Codewars Katas</h1>

<h6 align="center">
  Solutions with tests, tips and tutorials for <a href="https://www.codewars.com">Codewars</a> katas
</h6>

<p align="center">
  <a href="https://github.com/sindresorhus/xo">
    <img src="https://img.shields.io/badge/code_style-XO-5ed9c7.svg?style=flat-square">
  </a>
  <a href="https://github.com/prettier/prettier">
    <img src="https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square">
  </a>
</p>

> Maintained by [Abul Hasan](https://github.com/ahasan09). Originally forked from [lndgalante/codewars-katas](https://github.com/lndgalante/codewars-katas) — thanks to Leonardo Galante for the excellent structure and tooling.

### Vocabulary

- **Kata**: an algorithm you have to solve in any programming language you desire
- **Kyu**: a digit that determines kata difficulty level as well as the user rank on the platform

### Requirements

- Node.js 20+ (CI runs on Node 20)
- Tests via [Jest](https://jestjs.io); linting via [XO](https://github.com/sindresorhus/xo); formatting via [Prettier](https://prettier.io); pre-commit hooks via [Husky](https://typicode.github.io/husky)

### Purpose

Practicing katas helps improve your algorithmic thinking. It can also help you walk into interviews more confident and teach you a few tricks of your preferred language.
The [Tech Interview Handbook](https://github.com/yangshun/tech-interview-handbook) is a great companion resource.

### Repository Structure

There's a folder for each kata nested in its own kyu:

```ascii
├── 8-kyu/
│   ├── Mr. Freeze/
│   │   ├── index.js
│   │   └── index.test.js
│   └── ...
│
├── 7-kyu/
│   ├── Binary Addition/
│   │   ├── index.js
│   │   └── index.test.js
│   └── ...
```

### Global Index

Katas ordered alphabetically with a link to each kata folder:

- [8 Kyu - Index](lib/index/8-kyu.md)
- [7 Kyu - Index](lib/index/7-kyu.md)
- [6 Kyu - Index](lib/index/6-kyu.md)
- [5 Kyu - Index](lib/index/5-kyu.md)

To regenerate the global index run:

```bash
npm run update-index
```

### Create a New Kata

The kata generator has its own dependencies — install them first:

```bash
npm run install-generator-deps
```

Then generate a new folder with an `index.js` and `index.test.js`:

```bash
npm run create-kata [kata link]

# example
npm run create-kata https://www.codewars.com/kata/drying-potatoes/train/javascript
```

Since this is a 7-kyu kata it will appear under that folder with its own title, "Drying Potatoes".

### Running Tests

```bash
npm test              # full suite (1000+ tests)
npm run test-watch    # watch mode for uncommitted files
npm run lint          # XO
```

### Tips

1. Katas have `tags` that can hint at what to use (e.g. regular expressions).
2. Katas can have issues beyond your implementation — if you're stuck, check the kata's `Issues` on Codewars.
3. Check the `Discuss` section when instructions aren't clear.
4. After submitting, study other solutions and iterate on your own.
5. To compare solution performance, use [JSBench](https://jsbench.me).

### Learning Resources

- [Regular Expressions — Eloquent JavaScript](https://eloquentjavascript.net/09_regexp.html) · [The Modern JavaScript Tutorial](https://javascript.info/regexp-introduction) · [Awesome RegEx](https://github.com/aloisdg/awesome-regex)
- [Modern JavaScript Cheatsheet](https://github.com/mbeaudru/modern-js-cheatsheet) · [Array Explorer](https://sdras.github.io/array-explorer) · [Object Explorer](https://sdras.github.io/object-explorer)
- [Clean Code JavaScript](https://github.com/ryanmcdermott/clean-code-javascript) · [30 Seconds of Code](https://github.com/Chalarangelo/30-seconds-of-code) · [JavaScript Algorithms and Data Structures](https://github.com/trekhleb/javascript-algorithms)

### Similar Platforms

[LeetCode](https://leetcode.com) · [HackerRank](https://www.hackerrank.com) · [Exercism](https://exercism.org) · [Codility](https://codility.com) · [CodeChef](https://www.codechef.com) · [CoderByte](https://coderbyte.com)

### License

MIT — original work © [Leonardo Galante](https://leonardogalante.com), fork maintained by Abul Hasan.
