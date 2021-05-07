# javascript-string-utils

#### Check if a word starts with uppercase: 

```
String.prototype.startsWithUpperCase = function() {

  return this.match(/[A-Z]/) != null ? true : false;
}
```

#### Captalize a string
```
String.prototype.captalize = function() {

  const lowerCased = this.toLowerCase();
  const captalizedFirstLetter = lowerCased[0].toUpperCase();
  const restOfTheWord = this.slice(1);

  return `${captalizedFirstLetter}${restOfTheWord}`;
}
```
