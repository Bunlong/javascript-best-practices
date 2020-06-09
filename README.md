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

#### The Ternary Operator

Amateur:

```js
let hungry = true;
let eat;
if (hungry) {
  eat = 'yes';
} else {
  eat = 'no';
}
```

Pro:

```js
let hungry = true;
let eat = hungry ? 'yes' : 'non';
```
