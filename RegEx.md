# RegEx (Regular Expressions)

## RegEx in JavaScript 
- to find all the matching patterns
```js
let matches = "text".match( regex code );
```
- to search for a single match
```js
let index = "text".search( regex code );
```
- to replace the text find by regex with new one
```js
let next = "text".replace( regex code , "text need to replace with" );
```

## Exercise for me to practice
## text :
Alice bought 3 apples, 5 bananas, and 12 oranges.
Her email is alice_wonder@domain.com.
She paid $24.50 at the store.
Website: http://shop.example.com
Phone: +1-202-555-0147

1 - Find all the numbers.
```
[0-9] or \d
```
2 - Extract the email address.
```
\w+@[a-zA-Z]+.com
```
3 - Extract the website URL.
```
http\S+.com
```
4 - Extract the price.
```
[$][\d.]+
```
5 - Extract the phone number.
```
[+][\d-]+
```
6 - Replace the email with [hidden].
```
str.replace(/\b\S+@[a-zA-Z]+.com\b/g , "")
```
7 - Split the sentence into words.
```
str.split(/\s/g)
```

