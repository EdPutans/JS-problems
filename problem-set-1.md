### Problem Set 1

#### 1. Iteration

Using only `for` loops, write each of the following methods

- a. A function that simulates `forEach`
- b. A function that simulates `map`
- c. A function that simulates `filter`
- d. A function that simulates `find`
- e. A function that simulates `reduce`
- f. A function that takes an object and creates an array of arrays using key-value pairs:

```
ex. 
{beef: "steak", age: 50, dog: {name: "Rover", breed: "Husky"}}

==>

[
	["beef", "steak"],
	["age", 50],
	["dog", {name: "Rover", breed: "Husky"}]
]
```

- g. Extend the above example so that it works on nested objects as well. Write it so that it can work on any nested object, no matter how deeply nested it is.

```
ex. 
{beef: "steak", age: 50, dog: {name: "Rover", breed: "Husky"}}

==>

[
	["beef", "steak"],
	["age", 50],
	["dog", [["name", "Rover"], ["breed", "Husky"]]]
]
```



#### 2. Objects

- a. Inspect the data below: 

```js
	let data = [
		{
			name: "Mr. Ruffles",
			species: "dog"
		},
		{
			name: "Felix",
			species: "cat"
		},
		{ 
			name: "Sir Woofington III",
			species: "dog"
		},
		{
			name: "Lord Banoonoo",
			species: "monkey"
		},
		{
			name: "Max",
			species: "dog"
		},
		{
			name: "Ziggy",
			species: "iguana"
		},
		{
			name: "Raptor",
			species: "canary"
		},
		{
			name: "Howard",
			species: "iguana"
		},
		{
			name: "Lemon",
			species: "cat"
		},
		{
			name: "Samuel",
			species: "monkey"
		},
		{
			name: "Joey",
			species: "iguana"
		}
	]
```

Write a function that takes this data as an argument and returns an object with a key for each unique species. Each key should point to an array containing all objects having that species. Each object should also be assigned a unique ID. (i.e. the first object in the array of dogs should have an id of 1, the next 2, etc.). This function should not be specific to this data set and should be written to accomodate any number of different spcies.

- b. Write a function that takes an array of sentences and returns an object in which the keys are all of the unique words in all of the sentences, with values of arrays pointing to objects containing both the index of the sentence that contained it and the index of the word within the sentence. Make sure to ignore punctuation and capitalization.

```
ex.

[
	"The happy cat lapped up the milk joyously.",
	"Happy but tired, the milk man joyously turned in to bed",
]

==> 

{
	the: [{sentence: 0, word: 0}, {sentence: 0, word: 5}, {sentence: 1, word: 4}],
	happy: [{sentence: 0, word: 1}, {sentence: 1, word: 0}],
	cat: [{sentence: 0, word: 2}],
	lapped: [{sentence: 0, word: 3}]
	...
	bed: [{sentence: 1, word: 10}]
}
```

- c. Take the above example and write a function that takes an array of sentences and returns an object containing data about that array of sentences.

```
[
	"The happy cat lapped up the milk joyously.",
	"Happy but tired, the milk man joyously turned in to bed",
]

==> 
{
	num_sentences: 2,
	num_words: 19,
	num_unique_words: 14,
	most_frequently use word: "the",
	alphabetized_words: ["bed", "cat", "happy", "in" ... , "up"],
	word_locations: <RETURN VALUE FROM ABOVE EXERCISE>
}
```
