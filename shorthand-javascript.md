##shorthand Javascript
> The below shorthand javascript code is used for javascript developer. i have written some shorthand code over the yeare. i hope it's help to code improvement

1. ```Math.floor()```
   
   // Longhand
   
   Math.floor(4.3) === 4 // true
   
   //shorthand
   
   ~~4.9 === 4 // true

2. ```Math.pow()```
   
   // Longhand

     Math.pow(2,3); //8
     Math.pow(2,2); //4
   
   // Shorthand
   
     2**3; //8
     2**2; //4
   
3. ```Joining Array```
   
   // Longhand
   
     const odd = [1, 3, 5];
     const nums = [2, 4, 6].concat(odd);
     console.log(nums); // [2, 4, 6, 1, 3, 5];
   
   // shorthand (using spread operator )
   
     const odd = [1, 3, 5];
     const num = [2, 4, 6, ...odd];
     console.log(nums); // [2, 4, 6, 1, 3, 5];
   
4. ```Cloning Array```
   
     // Longhand
   
     const arr = [1, 2, 3, 4];
     const arra.slice();

     //  Shorthand
     const arr = [1, 2, 3, 4];
     const arr2 = [...arr];
   
5. ```Loop Array```
   
     // Longhand
   
     const fruits = [ 'mango', 'peach', 'banana'];
   
     for(let i = 0; i < fruits.length; i++);

     // Shorthand
   
     for ( let fruit of fruits)
   
     // if you wanted to access index, do
   
     for (let index in  fruits)
   
6. ```Ternary Operator```
   #Longhand
   	```sh
		const xy = 120;
		let answer;	
		if(xy > 120) {
			answer = 'if answer';
		} else {
			answer = 'else answer';
		}
	```
	#Shorthand
	```sh
		const answer = xy > 120 ? 'if answer' : 'else answer';
 	```
	#Nested If
	```sh
		const answer = xy > 120 ? 'First yes' : xy < 60 ? : 'Second yes' : 'No';
 	```
 7. ```swap function```
    
    	** Longhand **
    
    	```sh
           var a =1;
	   var b =2;
	   var temp = a;
	   a = b;
	   b = temp;
	   console.log(a,b); // 2,1
    	```
    
    	** Shorthand **
    
    	```sh
    	   var a = 1;
	   var b = 2;
	   [b,a] = [a,b];
	   console.log(a,b); // 2,1
    	```
