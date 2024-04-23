##shorthand Javascript
1. ```Math.floor()```
   
   // Longhand
   
   Math.floor(4.3) === 4 // true
   
   //shorthand
   
   ~~4.9 === 4 // true

3. ```Math.pow()```
   
   // Longhand

     Math.pow(2,3); //8
     Math.pow(2,2); //4
   
   // Shorthand
   
     2**3; //8
     2**2; //4
   
5. ```Joining Array```
   
   // Longhand
   
     const odd = [1, 3, 5];
     const nums = [2, 4, 6].concat(odd);
     console.log(nums); // [2, 4, 6, 1, 3, 5];
   
   // shorthand (using spread operator )
   
     const odd = [1, 3, 5];
     const num = [2, 4, 6, ...odd];
     console.log(nums); // [2, 4, 6, 1, 3, 5];
   
7. ```Cloning Array```
   
     // Longhand
   
     const arr = [1, 2, 3, 4];
     const arra.slice();

     //  Shorthand
     const arr = [1, 2, 3, 4];
     const arr2 = [...arr];
   
9. ```Loop Array```
   
     // Longhand
     const fruits = [ 'mango', 'peach', 'banana'];
     for(let i = 0; i < fruits.length; i++);

     // Shorthand
     for ( let fruit of fruits)
   
     // if you wanted to access index, do
     for (let index in  fruits)
   
10. 
