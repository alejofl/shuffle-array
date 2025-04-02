# @alejofl/shuffle-array (Class 2 Example)

> A small library that takes an array as input and returns a new array that is shuffled.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
   - [Examples](#examples)
- [Contribution](#contribution)
- [Security](#security)
- [License](#license)

## Installation

Install via npm:

```bash
npm install @alejofl/shuffle-array
```

Install via yarn:

```bash
yarn add @alejofl/shuffle-array
```

## Usage

Basic Usage

```js
import { shuffleArray } from '@alejofl/shuffle-array';

const startArray = [1, 2, 3, 4, 5];
const newShuffledArray = shuffleArray(startArray);

console.log(startArray);       // e.g., [1, 2, 3, 4, 5]
console.log(newShuffledArray); // e.g., [3, 1, 5, 2, 4]
```

### Examples

Shuffle a list of user IDs:

```js
import { shuffleArray } from '@alejofl/shuffle-array';

const userIds = ['u1', 'u2', 'u3', 'u4'];
const randomizedOrderOfUserIds = shuffleArray(userIds);

console.log(randomizedOrderOfUserIds); // e.g., ['u1', 'u3', 'u4', 'u2']
```

Use in a game for randomizing cards:

```js
import shuffleArray from '@alejofl/shuffle-array';

const deck = ['Ace of Spades', 'Two of Hearts']; // some card deck
const shuffledDeck = shuffleArray(deck);

console.log(shuffledDeck); // e.g., ['Two of Hearts', 'Ace of Spades', ...]
```

Use in a quiz application to randomize questions:

```js
import { cryptoShuffleArray } from '@alejofl/shuffle-array';

const questions = [
   { question: 'What is 2 + 2?', answer: 4 },
   { question: 'What is the capital of France?', answer: 'Paris' },
   { question: 'What is the chemical symbol for gold?', answer: 'Au' },
   { question: 'Who wrote "Romeo and Juliet"?', answer: 'William Shakespeare' }
];
const randomizedQuestions = cryptoShuffleArray(questions);

console.log(randomizedQuestions);
```

## Contribution

Contributions are welcome! Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for more details.

## Security

Please refer to our [SECURITY.md](./SECURITY.md) for information about our security policies, how to report vulnerabilities, and our approach to handling security concerns.

**Important Note**: This library offers both non-cryptographic randomness (`Math.random()`) and cryptographic randomness (`crypto` package).

## License

This project is licensed under the [MIT License](./LICENSE.md).

## Final Remarks

This project was done in an academic environment, as part of the curriculum of **Continuous Integration from University of Applied Sciences Technikum Wien (UASTW)**. The project was carried out by Alejo Flores Lucey (ID: if24x390).