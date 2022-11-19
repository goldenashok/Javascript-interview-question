1. way to create object

2. ```Object.preventExtensions()``` vs ```Object.seal()``` vs ```Object.freeze()```
    > Note: ```Use strict`` mode to throw an error when trying to modify an immutable object!
    - ```Object.preventExtensions()``` used to prevent additions of properties
    
    
            const person = {
                name: "ashok"
            }
            Object.preventEntensions(person);
            person.age = 33;
            console.log(person.age); // undefied
            
   - ```Object.seal()``` used to prevent addition and deletion of properties
           ```sh
           const person = {
                name: "ashok"
            }
            Object.seal(person);
            pesion.age = 33;
            delete pesion.name;
            console.log(pesion.age, persion.name); // undefined, ashok
           ```
   - ```Object.freeze()``` used to prevent addiition, deletion and modifying the properties
        ```sh
        const person = {
            name: "ashok"
        }
        Object.freeze(person);
        person.age = 33;
        person.name = "kumar";
        delete persion.name;
        console.log(person.age, peson.name); // undefied, ashok
        ```
