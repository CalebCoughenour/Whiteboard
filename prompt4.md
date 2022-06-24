write algorithm that determines whether all elements in string are unique
may not convert string to array 
return boolean

1. write function taking in string
2. loop through each element in string (i)
3. add second loop for each element string (j)
4. add conditional checking that i != j && string(i) != string(j)
5. if true, return true
6. return false if condition is not met


function uniqueCheck(string) {
  let bool = false;
  for (let i = 0; i < string.length; i++) {
    for(let j = 0; j < string.length; j++) {
      if (i != j && string(i) === string(j)) {
        return true;
      }
    }
  }
  return bool;
}