##shorthand Javascript
> The below shorthand javascript code is used for javascript developer. i have written some shorthand code over the yeare. i hope it's help to code improvement

1. ```Math.floor()```
   #### Longhand
    ```sh 
    Math.floor(4.3) === 4 // true
    ```
   #### shorthand
   ```sh
    ~~4.9 === 4 // true
    ```
2. ```Math.pow()```
   #### Longhand
     ```sh
    Math.pow(2,3); //8
     Math.pow(2,2); //4
   ```
   #### Shorthand
    ```sh
     2**3; //8
     2**2; //4
   ```
3. ```Joining Array```
   
   #### Longhand
   ```sh
    const odd = [1, 3, 5];
    const nums = [2, 4, 6].concat(odd);
    console.log(nums); // [2, 4, 6, 1, 3, 5];
   ```
   #### shorthand (using spread operator )
   ```sh
    const odd = [1, 3, 5];
    const num = [2, 4, 6, ...odd];
    console.log(nums); // [2, 4, 6, 1, 3, 5];
   ```
4. ```Cloning Array```
    #### Longhand
   ```sh
    const arr = [1, 2, 3, 4];
    const arra.slice();
    ```
    #### Shorthand
    ```sh
    const arr = [1, 2, 3, 4];
    const arr2 = [...arr];
   ```
5. ```Loop Array```
   #### Longhand
   ```sh
    const fruits = [ 'mango', 'peach', 'banana'];
    for(let i = 0; i < fruits.length; i++);
    ```
    #### Shorthand
    ```sh
    for ( let fruit of fruits)
   ```
    #### if you wanted to access index, do
   ```sh
    for (let index in  fruits)
   ```
6. ```Ternary Operator```
   #### Longhand
   	```sh
	const xy = 120;
	let answer;	
	if(xy > 120) {
		answer = 'if answer';
	} else {
		answer = 'else answer';
	}
	```
	#### Shorthand
	```sh
	const answer = xy > 120 ? 'if answer' : 'else answer';
 	```
	#### Nested If
	```sh
	const answer = xy > 120 ? 'First yes' : xy < 60 ? : 'Second yes' : 'No';
 	```
 7. ```swap function```
    #### Longhand
	```sh
	 var a =1;
	 var b =2;
	 var temp = a;
	 a = b;
	 b = temp;
	 console.log(a,b); // 2,1
	```
    #### Shorthand
    ```sh
    var a = 1;
    var b = 2;
    [b,a] = [a,b];
    console.log(a,b); // 2,1
    ```
8. ```Destructuring for multiple value ```
    #### Longhand
    ```sh
    function margin() {
	  var left=1, right=2, top=3, bottom=4;
	  return { left: left, right: right, top: top, bottom: bottom };
	}
	var data = margin();
	var left = data.left;
	var bottom = data.bottom;
	console.log(left, bottom); // 1 4
    ```
    #### Shorthand
    ```sh
    function margin() {
	  const left=1, right=2, top=3, bottom=4;
	  return { left, right, top, bottom };
	}
	const { left, bottom } = margin();
	console.log(left, bottom); // 1 4
    ```
9. ```Declaring the variable```
    #### Longhand
    ```sh
    let x;
	let y;
	let z = 3;
    ```
    #### Shorthand
    ```sh
    let x,y,z=3;
    ```
10. ```Object Property```
    #### Longhand
    ```sh
    const x = 20, y = 30;
	const obj = {x:x,y:y};
    ```
    #### Shorthand
    ```sh
    const x = 20, y = 30;
	const obj = {x,y};
    ```
11. ```Arrow function```
    #### Longhand
    ```sh
    function sayHello(name) {
		console.log('Hello', name);
	}

	setTimeout(function() {
	  console.log('Loaded')
	}, 2000);

	list.forEach(function(item) {
	  console.log(item);
	});
    ```
    #### Shorthand
    ```sh
    sayHello = name => console.log('Hello', name);
	setTimeout(() => console.log('Loaded'), 2000);
	list.forEach(item => console.log(item));
    ```
12. ```Implicit Return```
    #### Longhand
    ```sh
    function calcCircumference(x,y) {
		return x * y
	}
    ```
    #### Shorthand
    ```sh
    calcCircumference = (x,y) => x*y;
    ```
13. ```Default Parameter```
    #### Longhand
    ```sh
    function defautlfun(l, w, h) {
		if(w === undefined) {
			w=3;
		}
		if(h === undefined) {
			h=4;
		}
		return l * w * h;
	}
	defautlfun(2); // 24
    ```
    #### Shorthand
    ```sh
    defautlfun(l, w=2, h=4) => (l*w*h);
	defautlfun(2); // 24
    ```
14. ```Template Litrals```
    #### Longhand
    ```sh
    var first = 'ashok';
	var second = 'kumar';	
	var welcome = 'welcome to '+first+' '+second+'.';
    ```
    #### Shorthand
    ```sh
    var first = 'ashok';
	var second = 'kumar';
	var welcome = `welcome to ${first} ${second}`;
	```
15. ```Destructuring assignment shorthand```
    #### Longhand
	```sh
    const observable = require('mobx/observable');
	const action = require('mobx/action');
	const runInAction = require('mobx/runInAction')
	```
	#### Shorthand
	```sh
	import { observable, action, runInAction } from 'mobx';
	const {store, from, loading, error} = this.props;
	```
16. ```Multiline String```
    #### Longhand
	```sh	
    var welcometxt = 'Lorem ipsum \n\t'
					+ 'Lorem ipsum \n\t'
					+ 'Lorem ipsum \n\t'
	```				
	#### Shorthand
	```sh
	var welcometxt = `Lorem ipsum
				Lorem ipsum
				Lorem ipsum.`
	```
17. ```Mandatory Parameter shorthand```
    #### ES5
	```sh
    function mandatory(testval) {
		if(testval === undefined) {
			throw new Error('Missing parameter!');
		}
		return testval;
	}
	```
	#### Es6
	```sh
    mandatorycheck = () => {
		throw new Error('Missing parameter');
	}
	
	mandatory = (testval = mandatorycheck()) => {
		return testval;
	}
	```
18. ```Arry.find Shorthand```
    ```sh
    const flowers = {
			{type: 'rose', color: 'red'},
			{type: 'sunflower', color: 'yellow'},
			{type: 'tulips', color: 'orange'}
		}
	```
	#### Longhand
	```sh
	function findFlowers() {
		for(let i=0; i<flowers.length; i++) {
			if(flowers[i].type === 'rose' && flowers[i].color === 'red') {
				return flowers[i];
			}
		}
	}
    ```
	#### Shorthand		
	```sh
	flowers.find(flower => flowers.type === 'rose' && flowers.name === 'red');
	```
19. ```Converting string to numebr```
    #### Es5
    ```sh
    const num1 = parseInt("100");
	const num2 = parseInt("100.01");
	```
	#### Shorthand
	```sh
	const num1 = +"100"; // converted to int
	const num2 = +"100.01"; // converted to flot
	```
