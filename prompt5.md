write an algorithm that sorts an array 
without using .sort()
sort the numbers from smallest to largest

1. write function that takes in array of numbers
2. loop through for length of array -1 (i)
3. add second loop for length of array -1 (j)
4. add conditional checking if  array[j] > array[j + 1]
5. if true save array[j] to temp variable, save array[j + 1] to array[j] and save temp to array[j + 1]
6. if not true move to next number
7. return array



function sort(array) {
  for (let i = 0; i < array.length - 1; i++){
    for (int j = 0; j < array.length - 1; j++) {
      if (array[j] > array[j + 1]) {
        let temp = array[j];
        array[j] = array[j + 1];
        array[j + 1] = temp;
      }
    }
  }
  return array;
}