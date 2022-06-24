<!-- I figured out during my prompt that this is a wrong approach, the prompt I did for my whiteboard I think is how the more correct solution would be -->


write an algorithm that removes duplicates from an array
do not use functions like "filter()"
after solving demonstrate the use of "filter()"

1. write a function that takes in array
2. loop through array (i) for length of array
3. add second loop that will compare (j) to (i) and also making sure array[i] != array[j]
4. if they are equal, and not the same position, remove from array
5. if not equal, move to next element
6. return altered array, removed duplicates



function removeDuplicates (inputArray) {
  for (let i = 0; i < inputArray.length; i++) {
    for (let j = 0; j < inputArray.length; i++) {
      if (inputArray[j] === inputArray[i] && j != i) {
        inputArray.splice(i, 1);
      }
    }
  }
  return inputArray;
}

function filterDuplicates (inputArray) {
  for (let i = 0; i < inputArray.length; i++) {
    for (let j = 0; j < inputArray.length; i++) {
      if (inputArray[j] === inputArray[i] && j != i) {
        inputArray.filter(e => inputArray[i]);
      }
    }
  }
  return inputArray;
}

const recursiveRemoveDuplicates = (inputArray) => {
  if(input[0] === input[1]) {
    return recursiveRemoveDuplicates()
  }
}