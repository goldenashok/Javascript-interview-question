Type of function

1. Named function
   Locally / Traditional way
   ```
   function myFunction() {
     console.log('CodeBustler');
   }
   ```
2. Anonymous Function
   Anonymous Functions | withouth name, used a function expression or a arguments
   ```
   let great = function(name) {
     console.log(`Hello ${name}`);
   }
   ```
3. Arrow Function
   Arrow Function introduced in ES6, shart syntax & one-lined function
   arrow functions do not have their own this context. Instead, they capture the this value from the surrounding lexical context in which the arrow function was created.
   ```
     let great = () => console.log("Hello");
     great();
   ```
4. IIF Function
   immediately invoked Function expressions (IIFE) Executed immediatly after their creation. used to create private scops and avoid polluting the global namespace
   ```
   (function() {
      let str = 'Good Evening';
      console.log(str);
   })();
   ```
5. Higher Order Function
   Function that take one or more functions as arguments or return a function.
   ex: map(), filter(), reduce()

   ```
      let newArray = arr.map((item) => element * 10);
      console.log(newArray);
   ```
6. Constructor Function
   used a bleuprints for creating objects with similar properties using the new keyword to create instance of objects.

   ```
      function Person(name, place) {
         this.name = name;
         this.place = place;
      }
      let user1 = new Person('CodeBustler', 'india');
      console.log(`Hellow everyone this is ${user1.name}`);
   ```
