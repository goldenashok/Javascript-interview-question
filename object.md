1. ```Object.preventExtensions()``` vs ```Object.seal()``` vs ```Object.freeze()```
    ```Object.preventExtensions()``` used to prevent additions of properties
    
    ```sh
    const person = {
        name: "ashok"
    }
    Object.preventEntensions(person);
    person.age = 33;
    console.log(person.age); // undefied
    ```
