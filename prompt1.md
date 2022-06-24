URLs can not have spaces
all spaces in a string are replaced with %20
write an algorith that replaces all spaces in a string with %20

May not use replace() methord or regular expressions



1. function takes in string, create new empty string to add chars to
2. add loop to go through each character
3. add conditional that checks if current element is an empty space/string " "
4. if condition is true, replace space with %20
5. if condition is false, move to next element
6. return new string



function replaceSpace(string) {
  resultString = "";
  for (let i = 0; i < string.length) {
    if (string[i] === " ") {
      resultString += "%20";
    } else {
      resultString += string[i];
    }
  }
  return resultString;
}


const recursiveReplaceString(string) {
  resultString = "";
  if (string[i] === " ") {
    resultString += "%20";
  } else {
    return recursiveReplaceString(resultString += string[i]);
  }
}