## Array Interview question
1. How to create Array

   There are 2 way to create Array
    - ```new Array()```

        ```sh
        let a = new Array();
        a['name'] = 'Ashok';
        console.log(a); // ['name': 'Asok']
        ```
     > Note: if you are creating Array with single parameter, it consider the parameter as length. passwing more then parameter consider as a value

        let a = new Array(10);
        console.log(a); // [length : 10];

        let b = new Array(10, 11);
        console.log(b); // [10, 11]

     - ```[]``` Advanced method

        ```sh
        let a = [];
        a['name'] = 'Ashok';
        console.log(a); // ['name': 'Asok']
        ```
2. Sort By Name Ascenting Order
   ```
   let passengerDetail = [
     {name: 'Ashok', age: 40, sex: 'male'},
     {name: 'Ajay', age: 35, sex: 'male'},
     {name: 'Raja', age: 33, sex: 'male'},
     {name: 'Raji', age: 28, sex: 'female'},
     {name: 'Nithya', age: 32, sex: 'female'},
     {name: 'Prasanth', age: 29, sex: 'male'}
   ];
   ```
   ```
   let sortName = passengerDetail.sort((x,y) => {
      if(x.name - y.namme) {
         return -1;
      }
   }
   ```
3. Sort By Name Decending Order
   ```
   let passengerDetail = [
     {name: 'Ashok', age: 40, sex: 'male'},
     {name: 'Ajay', age: 35, sex: 'male'},
     {name: 'Raja', age: 33, sex: 'male'},
     {name: 'Raji', age: 28, sex: 'female'},
     {name: 'Nithya', age: 32, sex: 'female'},
     {name: 'Prasanth', age: 29, sex: 'male'}
   ];
   ```
   ```
   let sortName = passengerDetail.sort((x,y) => {
      if(y.name - x.namme) {
         return -1;
      }
   }
   ```
4. Sort by Age Acenting Order
   ```
      let passengerDetail = [
     {name: 'Ajay', age: 40, sex: 'male'},
     {name: 'Ashok', age: 35, sex: 'male'},
     {name: 'Raja', age: 33, sex: 'male'},
     {name: 'Raji', age: 28, sex: 'female'},
     {name: 'Nithya', age: 32, sex: 'female'},
     {name: 'Prasanth', age: 29, sex: 'male'}
   ];
   ```
   ```
   let sortByAge = passengerDetail.sort((x, y) => {
     return x.age - y.age;
   });
   ```
