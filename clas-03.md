# React List and Keys

**Lists are an important aspect within your app. Every application is bound to make use of lists in some form or the other. You could have a list of tasks like a calendar app, list of pictures like Instagram, list of items to shop in a shopping cart and so on. The use-cases are numerous.**

**_Lists within an application can be performance heavy._**
**Imagine an app with a huge list of videos or pictures and you keep getting thousands more, as you scroll. That could take a toll on the appβs performance.**
**Because performance is an important aspect, when you are using lists you need to make sure they are designed for optimal performance.**

**in React, when use lists, each list item needs a unique key**.

**the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it**.

## Spread Operator

**the spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a functionβs arguments.**
_it`s refers to the use of an ellipsis of three dots **(β¦)** to expand an iterable object into the list of arguments._

### **The Use Of It**

* **Copying an array**
* **Concatenating or combining arrays**
* **Using Math functions**
* **Using an array as arguments**
* **Adding an item to a list**
* **Adding to state in React**
* **Combining objects**
* **Converting NodeList to an array**

### Combining Objects Example

**The spread syntax is useful for combining the properties and methods on objects into a new object:**

`const objectOne = {hello: "π€ͺ"}`
`const objectTwo = {world: "π»"}`
`const objectThree = {...objectOne, ...objectTwo, laugh: "π"}
console.log(objectThree) // Object { hello: "π€ͺ", world: "π»", laugh: "π" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("π".repeat(5))}}
objectFour.laugh() // πππππ`

## **Using an array as arguments**

Since the spread operator βspreadsβ an array into different arguments, any functions that accepts multiple any number of arguments can benefit from use of the spread operator.

`const fruitStand = ['π','π','π']
`const sellFruit = (f1, f2, f3) => { console.log(`Fruits for sale:` ${f1}, ${f2}, ${f3}`) }`
`sellFruit(...fruitStand) // Fruits for sale:` π, π, π
`fruitStand.pop()`
`fruitStand.pop()`
`fruitStand.push('π')`
`fruitStand.push('π')`
`sellFruit(...fruitStand) // Fruits for sale: π, π, π`
`fruitStand.pop()`
`fruitStand.pop()`
`sellFruit(...fruitStand,'π') // Fruits for sale:` ``π, π,undefined``

## **Adding an item to a list**

**Asnoted in the last example, the spread operator can add an item to an another array with a natural, easy-to-understand syntax:**

`const fewFruit = ['π','π','π']`
`const fewMoreFruit = ['π', 'π', ...fewFruit]`
`console.log(fewMoreFruit) //  Array(5) [ "π", "π",`"π", "π", "π" ]`
