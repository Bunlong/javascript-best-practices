# JavaScript Best Practices

### JavaScript Tricks

#### Number to string / String to number

Amateur:

```js
let num = 15;
let s = num.toString(); // number to string
let n = Number(s); // string to number
```

Pro:

```js
let num = 15;
let s = num + ''; // number to string
let n = + s; // string to number
```
