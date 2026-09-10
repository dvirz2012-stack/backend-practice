# backend-practice

JSON:
JSON is a text format: it is a lightweight data interchange format that is easy for humans to read and write
and easy for machines to parse and generate, it is often used for transmitting data in web applications between a server and a
client.

JSON is built on two structures:
  1. A collection of value/name pairs. aka in other languages an object, record, struct, dictionary, hash table, keyed list, or       associative array.
  2. An ordered list of values. in most languages, its known as an array, list, vector or sequence.
these are universal data structures. virtually all programming languages support them in one way or another. it makes sense that a
data format that is interchangeable with programming languages also be based on these structures.

and object is an unordered set of name/value pairs. An object begins with a { and ends with a } , each name is followed by a colon :
and the name/value pairs are seperated with a , comma.

(I tried my best on these graphs)...
Object:
  { ---> whitespace ---------------------------- } -->
     |                                         |
    ,--> whitespace --> string --              |
    |                            |             |
    |        ____________________|             |
    |        |_____whitespace --> : --> value--|
    |----------------------------------------- |

Array:
  [ ---> whitespace ---------------------------- ] -->
     |                                       |
    ,--> value ------------------------------
    |                                        |
    |________________________________________|


async / await execution order

in JS theres a function called an async function:
```js
  async function x(){
    return 1;
  }
```
