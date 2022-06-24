write an algorithm that takes a string with repeated characters
compress the repeated characters using a number to show how many times it was repeated
i.e. aaa = 3a

1. write function taking in string, create counter int and empty result string
2. loop through string for length of string (i), add counter reset for each time loop moves to next element
3. add second loop for string (j)
4. add conditional comparing string(i) to string(j) and checking that i != j
5. if condition is true add to counter +1 for each equal letter, remove string(j) and add string(i) to result string
6. if condition is false push letter to result string
7. return result string


function compressString(string) {
  stringArray = string.map();
  tempArray = []
  resultString = "";
  for (let i = 0; i < stringArray.length; i++){
    for (let j = 0; j < stringArray.length; j++) {
      if (j != i && stringArray[i] === stringArray[j])
      {
        stringArray.pop(stringArray[j])
        tempArray.push(stringArray[i])
      } else {
          resultString += stringArray[i];
      }
    }
  }
  return resultString;
}