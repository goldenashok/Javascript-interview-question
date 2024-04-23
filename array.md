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
