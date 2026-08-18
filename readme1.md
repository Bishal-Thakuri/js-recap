## 1. What is the output?

const numbers = [1, 2, 3];
const result = numbers.map(n => n \* 5);
console.log(result);
console.log(numbers);

[5,10,15]
[1,2,3]

## 2. What is the output?

const numbers = [10, 15, 20, 25, 30];
const result = numbers.filter(n => n >= 20);
console.log(result);

[20,25,30]

## 3. What is the output?

const numbers = [5, 10, 15, 20];
const result = numbers.find(n => n > 10);
console.log(result);

15

## 4. What is the output?

const numbers = [1, 2, 3, 4];
const result = numbers.reduce((total, n) => total + n, 0);
console.log(result);

10

## 5. What is the output?

const students = [
{ name: "Ram", age: 17 },
{ name: "Hari", age: 20 },
{ name: "Kedar", age: 22 }
];

const result = students
.filter(student => student.age >= 18)
.map(student => student.name);

console.log(result);

Hari
Kedar

==============================

## Challenge 1 — Find expensive products

const products = [
{ name: "Laptop", price: 75000 },
{ name: "Mouse", price: 1500 },
{ name: "Phone", price: 50000 },
{ name: "Keyboard", price: 3000 }
];

const expensive = products.filter(product => product.price > 10000);

console.log(expensive);

========Output=========
[
{name: "Laptop", price: 75000},
{name: "Phone", price: 50000}
]

## Challenge 2 — Get product names

const products = [
{ name: "Laptop", price: 75000 },
{ name: "Mouse", price: 1500 },
{ name: "Phone", price: 50000 }
];

const names = products.map(product => product.name);

console.log(names);

========Output=========
["Laptop","Mouse","Phone"]

## Challenge 3 — Find a specific product

const products = [
{ id: 1, name: "Laptop" },
{ id: 2, name: "Phone" },
{ id: 3, name: "Mouse" }
];

const product = products.find(product => product.id === 2);

console.log(product);
console.log(product.name);

========Output=========
{ id: 2, name: "Phone" }
Phone

## Challenge 4 — Calculate total price

const products = [
{ name: "Laptop", price: 75000 },
{ name: "Phone", price: 50000 },
{ name: "Mouse", price: 1500 }
];

const total = products.reduce(
(sum, product) => sum + product.price,
0
);

console.log(total);

========Output=========
126500

## Challenge 5 

const users = [
{ name: "Ram", age: 17, active: true },
{ name: "Hari", age: 22, active: false },
{ name: "Kedar", age: 23, active: true },
{ name: "Sita", age: 16, active: true }
];

const result = users
.filter(user => user.age >= 18)
.filter(user => user.active)
.map(user => user.name);

console.log(result);

========Output=========
["Kedar"]

## Challenge 6 

const numbers = [1, 2, 3, 4, 5];

const result = numbers
.filter(n => n % 2 === 0)
.map(n => n \* 10)
.reduce((sum, n) => sum + n, 0);

console.log(result);

========Output=========
60

===================================

## AGAIN CHALLENGE

===================================

## Challenge 1

const numbers = [2, 5, 8, 11, 14, 17];

const result = numbers
.filter(n => n > 7)
.map(n => n \* 2);

console.log(result);

[16,22,28,34]

## Challenge 2

const users = [
{ name: "Ram", age: 16 },
{ name: "Hari", age: 21 },
{ name: "Kedar", age: 25 }
];

const user = users.find(user => user.age > 18);

console.log(user.name);

Hari

## Challenge 3

const numbers = [10, 20, 30];

const result = numbers.reduce((sum, n) => {
return sum + n;
}, 100);

console.log(result);

160

## Challenge 4 

const products = [
{ name: "Laptop", price: 75000 },
{ name: "Mouse", price: 1500 },
{ name: "Phone", price: 50000 },
{ name: "Keyboard", price: 3000 }
];

const result = products
.filter(product => product.price >= 5000)
.map(product => product.price)
.reduce((total, price) => total + price, 0);

console.log(result);

125000

## Challenge 5 

const students = [
{ name: "Ram", marks: 45 },
{ name: "Hari", marks: 75 },
{ name: "Kedar", marks: 90 },
{ name: "Sita", marks: 60 }
];

const result = students
.filter(student => student.marks >= 60)
.map(student => student.name);

console.log(result);

["Hari","kedar","Sita"]


## 1.What is an array of objects?

Array containing objects as element is known as array of objects.
or
An array of objects is an array where each element is an object containing key-value pairs.

## 2.What is the difference between for...of and forEach()?

for...of iterates directly over the value.
forEach() takes a callback function.
or
for...of is a loop that directly iterates over iterable values, while forEach() is an array method that executes a callback function for each element.

== imp difference ==
for...of can use:break and continue But you cannot directly use break or continue inside forEach().

## 3.What does map() return?

map returns new array

== imp detail ==
map() returns a new array with the result of the callback for every element.

## 4.What is the difference between find() and filter()?

find() returns the first matching element.
filter() returns all matching elements in a new array.
or
find() returns the first element that satisfies a condition, while filter() returns all elements that satisfy the condition as a new array.

## 5.Why is map() heavily used in React?

map() is heavily used because React needs to render a list of data into multiple components/elements.
or
map() is heavily used in React because it allows us to transform an array of data into a list of React elements or components.

## 6.What is destructuring?

Destructuring is a JavaScript syntax that allows us to extract values from arrays or properties from objects and assign them to variables.
or
Destructuring allows us to extract values from arrays or properties from objects and store them directly in variables.

## 7.What is the spread operator?

It means expanding/ spreading the elements or properties.

## 8.Why do React developers use the spread operator so often?

The major reason is immutability and creating updated copies of state/objects.
or
React developers frequently use the spread operator to create new copies of arrays or objects while updating state without directly mutating the original data.

## 9.What's the difference between spread and rest when both use ...?

spread operators expands existing values:
rest operators collects multiple values:

## 10,What is the output?

const numbers = [1, 2, 3, 4];

const result = numbers
.filter(n => n % 2 === 0)
.map(n => n \* 5);

console.log(result);

output=[10,20]
