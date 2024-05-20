1. Ordinal Program
  ```
  function getNumberWithOrdinal(n) {
  var s = ["th", "st", "nd", "rd"],
      v = n % 100;
  return n + (s[(v - 20) % 10] || s[v] || s[0]);
  }
  
  [-4,-1,0,1,2,3,4,10,11,12,13,14,20,21,22,100,101,111].forEach(
    n => console.log(n + ' -> ' + getNumberWithOrdinal(n))
  );
  ```
2. Find Duplicate Value in the given Array
  ```
  const counts = {};
  const sampleArray = ['a', 'a', 'b', 'c'];
  sampleArray.forEach(function (x) { counts[x] = (counts[x] || 0) + 1; });
  console.log(counts);
  ```
  Output :
  ``` {a: 2, b:1, c:1} ```
 
