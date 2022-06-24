write an algorithm that takes a string with repeated characters
compress the repeated characters using a number to show how many times it was repeated
i.e. aaa = 3a

1. write function taking in string, create empty result string and map string to array
2. loop through string for length of string (i), add counter that resets each time loop moves to next element and add variable for current element
3. add while loop for length of array that counts occurences of element i
4. add conditional that will push current letter and count to result string if true
5. if condition is false push letter to result string
6. return result string


function compressString(string) {
  stringArray = string.map();
  resultString = "";
  for (let i = 0; i < stringArray.length; i++){
    let count = 1;
    let  currentLetter = stringArray[i];
    while (i < stringArray.length - 1 && stringArray[i] === stringArray[i + 1]) {
        count++;
        i++;
      }
      if (count === 1) {
        resultString += currentLetter;
      } else {
        resultString += currentLetter + count;
      }
    }
  }
  return resultString;
}

