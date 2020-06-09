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

#### Dynamic Properties in Objects

Amateur:

```js
let dynamic = 'value';
let user = {
  id: 1
};
user[dynamic] = 'other value';
```

Pro:

```js
let dynamic = 'value';
let user = {
  id: 1,
  [dynamic] = 'other value'
};
```

#### Array to Object

Amateur:

```js
let arr = ['value1', 'value2', 'value3'];
let arrObject = {};
for (let i = 0; i < arr.length; ++i) {
  if (arr[i] !== undefined) {
    arrObject[i] = arr[i];
  }
}
```

Pro:

```js
let arr = ['value1', 'value2', 'value3'];
let arrObject = {...arr};
```
