## Object Interview Question

1. way to create object
    There are 2 way to create Object
    - ```new Object()```
    
            let a = new Object();
            a.name = 'ashok';
            
    - ```{}```
    
            let a = {};
            a.name = 'ashok'
           

2. ```Object.preventExtensions()``` vs ```Object.seal()``` vs ```Object.freeze()```
    > Note: ```Use strict``` mode to throw an error when trying to modify an immutable object!
    - ```Object.preventExtensions()``` used to prevent additions of properties
    
            const person = {
                name: "ashok"
            }
            Object.preventExtensions(person);
            person.age = 33;
            console.log(person.age); // undefied
            
   - ```Object.seal()``` used to prevent addition and deletion of properties
   
           const person = {
                name: "ashok"
            }
            Object.seal(person);
            pesion.age = 33;
            delete pesion.name;
            console.log(pesion.age, persion.name); // undefined, ashok
           
   - ```Object.freeze()``` used to prevent addiition, deletion and modifying the properties
        
            const person = {
                name: "ashok"
            }
            Object.freeze(person);
            person.age = 33;
            person.name = "kumar";
            delete persion.name;
            console.log(person.age, peson.name); // undefied, ashok

