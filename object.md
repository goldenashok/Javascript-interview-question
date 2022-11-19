1. ```Object.preventExtensions()``` vs ```Object.seal()``` vs ```Object.freeze()```
    - ```Object.preventExtensions()``` used to prevent additions of properties
    
    ```sh
    const person = {
        name: "ashok"
    }
    Object.preventEntensions(person);
    person.age = 33;
    console.log(person.age); // undefied
    ```
   - ```Object.seal()``` used to prevent additon and deletion of peroperties
   
   ```sh
   const person = {
        name: "ashok"
    }
    Object.seal(person);
    pesion.age = 33;
    delete pesion.name;
    console.log(pesion.age, persion.name); // undefined, ashok
   ```
