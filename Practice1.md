Write all the code inside main.js file

1. Create an empty class named Surgeon.

2. Inside the Surgeon class, create a constructor() method that accepts two parameters: name and department.

3. Inside the Surgeon constructor(), create name and department properties and set them equal to your input parameters.

4. Create an instance of the Surgeon class — set the name to 'Francisco Romero' and department to 'Cardiovascular'.

Save the instance to a constant variable called `surgeonRomero`.

5. Create an instance of the Surgeon class — set the name to 'Ruth Jackson' and department to 'Orthopedics'.

Save the instance to a constant variable called `surgeonJackson`.

6. In the Surgeon constructor, prepend the name and department properties with an underscore (`_`).

7. Inside of the constructor(), add a property named `_remainingVacationDays` and set it equal to 20.

8. Under the constructor(), create a getter called `name` that returns the value saved to `_name`.

9. Under the `name` getter, create a getter called `department` that returns the value saved to `_department`.

10. Under the `department` getter, create a getter called `remainingVacationDays` that returns the value saved to `_remainingVacationDays`.

11. Under the `remainingVacationDays` getter, create a method called `takeVacationDays` that accepts one argument named `daysOff`.

Inside of the method, subtract daysOff from the number saved to `_remainingVacationDays`. Set `_remainingVacationDays` to the result.

12. At the bottom of main.js, use console.log() to print the value saved to the `name` property of the `surgeonRomero` object.

13. Call `.takeVacationDays()` on `surgeonRomero`, with an input of `3`.

14. After the call to `.takeVacationDays()`, use `console.log()` to print the value saved to the `remainingVacationDays` property of the `surgeonRomero` instance.

# Inheritance

1. In the next few exercises, you will create two subclasses `(Doctor and Nurse)` from a parent class named `HospitalEmployee`.

Below, we have listed the properties and methods you will find in the `Doctor` and `Nurse` classes.

### Doctor

Properties: `_name`, `_remainingVacationDays` (set to 20 inside the constructor()), `_insurance`
Methods: `.takeVacationDays()`

### Nurse

Properties: `_name`, `_remainingVacationDays` (set to 20 inside constructor()), `_certifications`
Methods: `.takeVacationDays()`, `.addCertification()`

In main.js, create a parent class named `HospitalEmployee`. Add a constructor with `name` as an argument.

2. Inside of the constructor(), set the instance’s `_name` to name and `_remainingVacationDays` to 20.

3. Under the constructor, create getters for your `_name` and `_remainingVacationDays` properties.

Inside the getter, return the property’s value.

4. Under the getters, add a method called `takeVacationDays`.

This method should accept one argument, called `daysOff`.

Inside the method, subtract `daysOff` from `_remainingVacationDays`. Save the result to `_remainingVacationDays`.

5. Next create the `Nurse` class as a child of the `HospitalEmployee` class. Remember the `Nurse` class has the following properties and methods:

### Nurse

Properties: `_name`, `_remainingVacationDays` (set to 20 inside constructor()), `_certifications`
Methods: `.takeVacationDays()`, `.addCertification()`
Under `HospitalEmployee`, create an empty class named `Nurse` that extends `HospitalEmployee`.

6. Inside the `Nurse` class, create a `constructor()` that accepts two arguments. Use the list of properties above to name these arguments.

7. In the Nurse constructor, call the parent’s constructor method and pass the appropriate value(s).

8. Inside of the Nurse constructor, and under `super`, set `_certifications`.

9. Under the `Nurse` class, create a new instance of Nurse and save it to a constant variable named `nurseOlynyk`. Pass in the following values for each property:

name: 'Olynyk'
certifications: ['Trauma', 'Pediatrics']

10. Call `.takeVacationDays()` with an input of `5` on your `nurseOlynyk` instance.

11. Under the method call, log the value saved to the `remainingVacationDays` property in `nurseOlynyk`.

12. Under the Nurse constructor(), add a getter that returns the value saved to the Nurse instance’s `_certifications`.

13. Add a method called `addCertification` under the `certifications` getter.

The method should accept one input (`newCertification`). Inside the method, use the push method to add the newCertification value to the nurse’s certifications array.

14. At the bottom of main.js call the `.addCertification()` method on `nurseOlynyk` with a parameter of `'Genetics'`.

Log the value saved to the `certifications` property of `nurseOlynyk`.

15. Inside of your `HospitalEmployee` class, create a static method called `generatePassword`. When it’s called, this method should return a random integer between zero and 10,000.

## Doctor Class

1. If you want extra practice with inheritance, take some time to create a `Doctor` class that inherits from `HospitalEmployee`. The properties and methods for the Doctor class are listed below:

### Doctor

properties: `_name`, `_remainingVacationDays` (set to 20 inside constructor()), `_insurance`
methods: `.takeVacationDays()`
