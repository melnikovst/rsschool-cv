# Stanislav Melnikov

## Junior+/Middle frontend developer

### You could contact me:

1. [telegram](https://t.me/pay2w8)
2. Email: melnikovstn@yandex.ru

## About Me (introduction):

Hi there! I started education in a January 2022. I am really impressed with modern web services and wanna to be a part of their development.
I really interested to learn a new technologies and improving my expertise. I am working as a Frontend developer about a half-year and good known how important is not to stop studiyng.

## Hard Skills:

- Main languages:
  - JavaScript
  - TypeScript
- Markdown/stylesheet:
  - HTML
  - CSS
  - SCSS
- Frameworks/Libraries:
  - React
  - Redux
  - RTK
  - MobX
  - Zustand
- Backend:
  - NodeJS
  - ExpressJS
  - MongoDB
- Assembly:
  - Webpack
  - Gulp

## My code example:

- Task: [4 kyu](https://www.codewars.com/kata/52742f58faf5485cae000b9a)

  Need to implement a function which formats a duration, given as a number of seconds, in a human-friendly way. The duration is expressed as a combination of years, days, hours, minutes and seconds.

```
function formatDuration (seconds) {
  if (seconds === 0) return 'now'
  const s = seconds % 60;
  const m = Math.floor((seconds / 60)) % 60;
  const h = Math.floor((seconds / (60 * 60))) % 24;
  const d = Math.floor((seconds / (24 * 60 * 60))) % 365;
  const y = Math.floor((seconds / (365 * 24 * 60 * 60)));

  const arr = [
                {v: s, t: 'second'},
                {v: m, t: 'minute'},
                {v: h, t: 'hour'},
                {v: d, t: 'day'},
                {v: y, t: 'year'}
              ];

  const matched = arr.map((x, i) => {
    const {v, t} = x;
    if(v === 1) {
      return `${v} ${t}`
    }
    if (v > 1) {
      return `${v} ${t}s`
    }
  }).reverse();

  const filtered = matched.filter(x => x !== undefined);

  if (filtered.length > 1) {
    const y = filtered[filtered.length - 1];
    return `${filtered.slice(0, filtered.length - 1).join(', ')} and ${y}`
  }
  return filtered[0]
}
```

## My projects:

- Simple web-store (in progress):
  - Stack: TypeScript, React.js, Redux Toolkit, SCSS (modules)
  - Repo (code): https://github.com/melnikovst/sb-market-catalog
  - Deploy: https://melnikovst.github.io/sb-market-catalog/
- Clock (simple widget for getting a time):
  - Stack: TypeScript, React.js, SCSS
  - Repo (code): https://github.com/melnikovst/clock
  - Deploy: https://melnikovst.github.io/clock/

## Courses:

- Web Developing on Yandex (gratuated);
- RS School Stage 1 (in progress);

## Languages:

- Russian Native
- English B1-B2
