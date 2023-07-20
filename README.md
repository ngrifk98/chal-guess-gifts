# Guess the Gifts Code Challenge

Welcome to the "Guess the Gifts" code challenge! In this challenge, you are given a wishlist containing all possible items, and a list of presents received. Your task is to determine which of the wishlisted items you might have received based on the attributes (size, clatters, and weight) of the presents.

## Problem Statement

You will be provided with two arrays:

1. `wishlist`: An array of objects representing the items on your wishlist. Each object has the following format:

```javascript
{ name: "toy car", size: "medium", clatters: "a bit", weight: "medium" }
```

2. `presents`: An array of objects representing the presents received. Each object has the following format:

```javascript
{ size: "small", clatters: "no", weight: "light" }
```

Your task is to write a JavaScript function called `guessGifts(wishlist, presents)` that returns an array of names of all wishlisted presents that match the attributes of any of the presents received.

## Rules

- Possible values for `size`: "small", "medium", "large"
- Possible values for `clatters`: "no", "a bit", "yes"
- Possible values for `weight`: "light", "medium", "heavy"
- Do not add any item more than once to the result.
- The order of names in the output doesn't matter.
- It's possible that multiple items from your wishlist have the same attribute values. If they match the attributes of one of the presents, add all of them.

## Example

```javascript
var wishlist = [
  { name: "Mini Puzzle", size: "small", clatters: "yes", weight: "light" },
  { name: "Toy Car", size: "medium", clatters: "a bit", weight: "medium" },
  { name: "Card Game", size: "small", clatters: "no", weight: "light" },
];

var presents = [
  { size: "medium", clatters: "a bit", weight: "medium" },
  { size: "small", clatters: "yes", weight: "light" },
];

guessGifts(wishlist, presents); // Output: ["Toy Car", "Mini Puzzle"]
```

## How to Use

1. Fork this repository or copy the code from the `guess-gifts.js` file.
2. Implement the `guessGifts(wishlist, presents)` function in your preferred JavaScript environment or online editor.
3. Run the function with sample inputs to check the correctness of your implementation.

Feel free to modify the example inputs and outputs to test other scenarios.

## Constraints

- The input arrays (`wishlist` and `presents`) will have at most 1000 elements each.
- The name of each item in the `wishlist` will be a non-empty string with a maximum length of 100 characters.
- The attribute values (`size`, `clatters`, and `weight`) will always be valid according to the given rules.

