# Closures:

function create() {
  var counter = 0;
  return {
    increment: function() {
    counter++;
    },
    print: function() {
      console.log(counter);
    }
  }
}
var c = create();
c.increment();
c.print();     // ==> 1

# use ful function

1 => charAt()	Returns the character at the specified index.
2 => concat()	Combines the text of two strings and returns a new string.
3 => forEach()	Calls a function for each element in the array.
4 => indexOf()	Returns the index within the calling String object of the first occurrence of the specified value, or -1 if not found.
5 => length()	Returns the length of the string.
6 => pop()	Removes the last element from an array and returns that element.
7 => push()	Adds one or more elements to the end of an array and returns the new length of the array.
8 => reverse()	Reverses the order of the elements of an array -- the first becomes the last, and the last becomes the first.
9 => sort()	Sorts the elements of an array.
10 => substr()	Returns the characters in a string beginning at the specified location through the specified number of characters.
11 => toLowerCase()	Returns the calling string value converted to lower case.
12 => toString()	Returns the string representation of the number's value.
13 => toUpperCase()	Returns the calling string value converted to uppercase.

