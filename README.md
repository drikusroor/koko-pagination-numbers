# Koko pagination numbers

A function to generate page numbers with dots in between for navigational purposes.

All credits go to [sarifconrati](https://gist.github.com/sarifconrati) who provided the [gist](https://gist.github.com/sarifconrati/9f64c69757a95f2a34f679e9a330f72a). See also this [gist](https://gist.github.com/kottenator/9d936eb3e4e3c3e02598) (original by [kottenator](https://gist.github.com/kottenator) for other implementations of this algorithm and for translations to other programming languages.

## Installation

Install using npm or yarn

```bash
npm install koko-pagination-numbers
```

or

```bash
yarn add koko-pagination-numbers
```

## Usage

The first parameter is the current page. The second parameter is the last page. The third (optional) parameter is the width, or the amount of page numbers between the dots and the current page number (default = 2).

```javascript
const getPageNumbers = require("koko-pagination-numbers");

const pageNumbers = getPageNumbers(7, 30);
// returns [1, "...", 5, 6, 7, 8, 9, "...", 30]

const widerPageNumbers = getPageNumbers(15, 30, 4);
// returns [1, "...", 11, 12, 13, 14, 15, 16, 17, 18, 19, "...", 30]
```
