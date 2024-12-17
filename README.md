# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript bug related to loose equality (==) comparisons. The bug arises from the fact that loose equality performs type coercion before comparison, which can lead to unexpected results.

## Bug Description

The provided JavaScript function `foo` uses loose equality (`==`) to compare two input values.  This can cause issues when comparing values of different types that are considered equal under loose equality but not under strict equality (`===`). For instance, `0 == false` evaluates to `true`, while `0 === false` evaluates to `false`. 

## How to reproduce the bug

1. Clone this repository.
2. Open `bug.js`.
3. Run the code. Note the unexpected result when comparing values like 0 and false, or "0" and 0.

## Solution

The solution involves replacing loose equality (`==`) with strict equality (`===`) to prevent type coercion and ensure accurate comparisons.

## License

This project is licensed under the MIT License - see the LICENSE file for details.