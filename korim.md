1.let greeting;
greetign = {};
console.log(greetign);
A: {}
B: ReferenceError: greetign is not defined
C: undefined
Answer: B
Explanation: In the code provided, there is a typographical error. The variable is declared as "greeting," but it is assigned a value under the name "greetign." Due to this misspelling, when you try to log the variable "greetign," JavaScript will throw a ReferenceError because "greetign" is not defined.


2.
function sum(a, b) {
  return a + b;
}

sum(1, "2");
A: NaN
B: TypeError
C: "12"
D: 3
Answer: D
JavaScript is a weakly typed language, so when you use the + operator to add values, it performs type coercion if the operands are of different types. In this case, 1 is a number, and "2" is a string. JavaScript will attempt to convert the string to a number and then add them together, resulting in 3



3. Write the correct answer from the following options and give an explanation (2-5 lines).
const food = ["🍕", "🍫", "🥑", "🍔"];
const info = { favoriteFood: food[0] };

info.favoriteFood = "🍝";

console.log(food);
A: ['🍕', '🍫', '🥑', '🍔']
B: ['🍝', '🍫', '🥑', '🍔']
C: ['🍝', '🍕', '🍫', '🥑', '🍔']
D: ReferenceError

The correct answer is A: ['🍕', '🍫', '🥑', '🍔'].

Explanation:
In this code, we first create an array food containing four emoji elements. Then, we create an object info with a property favoriteFood that initially references the first element of the food array, which is "🍕".

Later in the code, we change the value of info.favoriteFood to "🍝", but this does not affect the food array in any way. The food array remains unchanged, and when we log it to the console, it will still contain the original elements "🍕", "🍫", "🥑", "🍔".


4. Write the correct answer from the following options and give an explanation (2-5 lines).
function sayHi(name) {
  return `Hi there, ${name}`;
}

console.log(sayHi());
A: Hi there,
B: Hi there, undefined
C: Hi there, null
D: ReferenceError

Answer 4: B - Hi there, undefined
Explanation: In the sayHi function, there is a parameter name which is expected to be passed when calling the function. However, when sayHi() is called without passing any argument, name is undefined. The template string includes this undefined value, resulting in "Hi there, undefined" being returned and logged to the console


5. Write the correct answer from the following options and give an explanation (2-5 lines).
let count = 0;
const nums = [0, 1, 2, 3];

nums.forEach((num) => {
  if (num) count += 1;
});

console.log(count);
A: 1
B: 2
C: 3
D: 4
Answer 5: C - 3
Explanation: The forEach method iterates over each element in the nums array. In this case, the callback function inside the forEach checks if num is truthy (i.e., not equal to 0). For the elements 1, 2, and 3 in the array, this condition is true, so the count variable is incremented for each of these elements. As a result, count becomes 3, and that value is logged to the console.

