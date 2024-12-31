### Answers:

1. **Rectangle class**

   ```javascript
   class Rectangle {
     constructor(width, height) {
       this.width = width;
       this.height = height;
     }
     area() {
       return this.width * this.height;
     }
     isLargerThan(otherRectangle) {
       return this.area() > otherRectangle.area();
     }
   }
   ```

2. **Counter class**

   ```javascript
   class Counter {
     constructor(initialValue = 0) {
       this.value = initialValue;
       this.initialValue = initialValue;
     }
     increment() {
       this.value++;
     }
     decrement() {
       this.value--;
     }
     reset() {
       this.value = this.initialValue;
     }
   }
   ```

3. **BankAccount class**

   ```javascript
   class BankAccount {
     constructor(balance = 0) {
       this.balance = balance;
     }
     deposit(amount) {
       this.balance += amount;
     }
     withdraw(amount) {
       if (amount <= this.balance) {
         this.balance -= amount;
       } else {
         console.log("Insufficient funds");
       }
     }
     getBalance() {
       return this.balance;
     }
   }
   ```

4. **Student class**

   ```javascript
   class Student {
     constructor(name, grades) {
       this.name = name;
       this.grades = grades;
     }
     averageGrade() {
       const sum = this.grades.reduce((a, b) => a + b, 0);
       return sum / this.grades.length;
     }
     hasPassed() {
       return this.averageGrade() >= 60;
     }
   }
   ```

5. **Car class**

   ```javascript
   class Car {
     constructor(make, model, year) {
       this.make = make;
       this.model = model;
       this.year = year;
     }
     carAge(currentYear) {
       return currentYear - this.year;
     }
     isClassic(currentYear) {
       return this.carAge(currentYear) > 25;
     }
   }
   ```

6. **ShoppingCart class**

   ```javascript
   class ShoppingCart {
     constructor() {
       this.items = [];
     }
     addItem(name, price, quantity) {
       this.items.push({ name, price, quantity });
     }
     removeItem(name) {
       this.items = this.items.filter((item) => item.name !== name);
     }
     calculateTotal() {
       return this.items.reduce(
         (total, item) => total + item.price * item.quantity,
         0
       );
     }
   }
   ```

7. **Person class**

   ```javascript
   class Person {
     constructor(name, age) {
       this.name = name;
       this.age = age;
     }
     static whoIsOlder(person1, person2) {
       if (person1.age > person2.age) {
         return `${person1.name} is older.`;
       } else if (person2.age > person1.age) {
         return `${person2.name} is older.`;
       } else {
         return "They are the same age.";
       }
     }
   }
   ```

8. **Queue class**

   ```javascript
   class Queue {
     constructor() {
       this.items = [];
     }
     enqueue(item) {
       this.items.push(item);
     }
     dequeue() {
       return this.items.shift();
     }
     display() {
       return this.items;
     }
   }
   ```

9. **Book class**

   ```javascript
   class Book {
     constructor(title, author, year) {
       this.title = title;
       this.author = author;
       this.year = year;
     }
     isOlderThan(years) {
       const currentYear = new Date().getFullYear();
       return currentYear - this.year > years;
     }
     displayInfo() {
       return `${this.title} by ${this.author}, published in ${this.year}`;
     }
   }
   ```

10. **Circle class**
    ```javascript
    class Circle {
      constructor(radius) {
        this.radius = radius;
      }
      area() {
        return Math.PI * this.radius ** 2;
      }
      circumference() {
        return 2 * Math.PI * this.radius;
      }
      isLargerThan(otherCircle) {
        return this.area() > otherCircle.area();
      }
    }
    ```
