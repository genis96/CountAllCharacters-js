# CountAllCharacters-js
Hack Reactor Module 1 Problem

// Hack Reactor Prep Module 1

/* Write a function called "countAllCharacters".

Given a string, "countAllCharacters" returns an object where each key is a character in the given string. The value of each key should be how many times each character appeared in the given string.

Notes:

If given an empty string, countAllCharacters should return an empty object.
var output = countAllCharacters('banana');
console.log(output); // --> {b: 1, a: 3, n: 2}
*/


/* My Pseudo Code 
1. create an object
2. itereate over the string
3. need to capture the specific word in string str[i] and must place it inside the new object and set it  to undefined 
4. make it start from 0 and return 0 if no string
5. Make it count now
6. Return object

*/

/* My Solution */

function countAllCharacters(str) {

    var newObjStr = {}; // (1)
    for(var i = 0; i < str.length; i++) { // (2)
        if(newObjStr[str[i]] === undefined) { // (3)
            (newObjStr[str[i]]) = 0; // (4)
        }
        newObjStr[str[i]]++; // (5)
    }
    return newObjStr; // (6)
}

var output = countAllCharacters('banana');
console.log(output); // --> {b: 1, a: 3, n: 2}
