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

# About Select

$('*'): This selector selects all elements in the document.

$("p > *"): This selector selects all elements that are children of a paragraph element.

$("#specialID"): This selector function gets the element with id="specialID".

$(".specialClass"): This selector gets all the elements that have the class of specialClass.

$("li:not(.myclass)"): Selects all elements matched by <li> that do not have class="myclass".

$("a#specialID.specialClass"): This selector matches links with an id of specialID and a class of specialClass.

$("p a.specialClass"): This selector matches links with a class of specialClass declared within <p> elements.

$("ul li:first"): This selector gets only the first <li> element of the <ul>.

$("#container p"): Selects all elements matched by <p> that are descendants of an element that has an id of container.

$("li > ul"): Selects all elements matched by <ul> that are children of an element matched by <li>

$("strong + em"): Selects all elements matched by <em> that immediately follow a sibling element matched by <strong>.

$("p ~ ul"): Selects all elements matched by <ul> that follow a sibling element matched by <p>.

$("code, em, strong"): Selects all elements matched by <code> or <em> or <strong>.

$("p strong, .myclass"): Selects all elements matched by <strong> that are descendants of an element matched by <p> as well as all elements that have a class of myclass.

$(":empty"): Selects all elements that have no children.

$("p:empty"): Selects all elements matched by <p> that have no children.

$("div[p]"): Selects all elements matched by <div> that contain an element matched by <p>.

$("p[.myclass]"): Selects all elements matched by <p> that contain an element with a class of myclass.

$("a[@rel]"): Selects all elements matched by <a> that have a rel attribute.

$("input[@name=myname]"): Selects all elements matched by <input> that have a name value exactly equal to myname.

$("input[@name^=myname]"): Selects all elements matched by <input> that have a name value beginning with myname.

$("a[@rel$=self]"): Selects all elements matched by <a> that have rel attribute value ending with self

$("a[@href*=domain.com]"): Selects all elements matched by <a> that have an href value containing domain.com.

$("li:even"): Selects all elements matched by <li> that have an even index value.

$("tr:odd"): Selects all elements matched by <tr> that have an odd index value.

$("li:first"): Selects the first <li> element.

$("li:last"): Selects the last <li> element.

$("li:visible"): Selects all elements matched by <li> that are visible.

$("li:hidden"): Selects all elements matched by <li> that are hidden.

$(":radio"): Selects all radio buttons in the form.

$(":checked"): Selects all checked boxex in the form.

$(":input"): Selects only form elements (input, select, textarea, button).

$(":text"): Selects only text elements (input[type=text]).

$("li:eq(2)"): Selects the third <li> element

$("li:eq(4)"): Selects the fifth <li> element

$("li:lt(2)"): Selects all elements matched by <li> element before the third one; in other words, the first two <li> elements.

$("p:lt(3)"): selects all elements matched by <p> elements before the fourth one; in other words the first three <p> elements.

$("li:gt(1)"): Selects all elements matched by <li> after the second one.

$("p:gt(2)"): Selects all elements matched by <p> after the third one.

$("div/p"): Selects all elements matched by <p> that are children of an element matched by <div>.

$("div//code"): Selects all elements matched by <code>that are descendants of an element matched by <div>.

$("//p//a"): Selects all elements matched by <a> that are descendants of an element matched by <p>

$("li:first-child"): Selects all elements matched by <li> that are the first child of their parent.

$("li:last-child"): Selects all elements matched by <li> that are the last child of their parent.

$(":parent"): Selects all elements that are the parent of another element, including text.

$("li:contains(second)"): Selects all elements matched by <li> that contain the text second.

You can use all the above selectors with any HTML/XML element in generic way. For example if selector $("li:first") works for <li> element then $("p:first") would also work for <p> element.


#Useful Attribute Methods:
Following table lists down few useful methods which you can use to manipulate attributes and properties:

Methods	Description
attr( properties )	Set a key/value object as properties to all matched elements.
attr( key, fn )	Set a single property to a computed value, on all matched elements.
removeAttr( name )	Remove an attribute from each of the matched elements.
hasClass( class )	Returns true if the specified class is present on at least one of the set of matched elements.
removeClass( class )	Removes all or the specified class(es) from the set of matched elements.
toggleClass( class )	Adds the specified class if it is not present, removes the specified class if it is present.
html( )	Get the html contents (innerHTML) of the first matched element.
html( val )	Set the html contents of every matched element.
text( )	Get the combined text contents of all matched elements.
text( val )	Set the text contents of all matched elements.
val( )	Get the input value of the first matched element.
val( val )	Set the value attribute of every matched element if it is called on <input> but if it is called on <select> with the passed <option> value then passed option would be selected, if it is called on check box or radio box then all the matching check box and radiobox would be checked.
