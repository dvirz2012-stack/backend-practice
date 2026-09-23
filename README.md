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
```text
Object:
  { ---> whitespace ---------------------------- } -->
     |                                         |
    ,--> whitespace --> string --              |
    |                            |             |
    |        ____________________|             |
    |        |_____whitespace --> : --> value--|
    |------------------------------------------|

Array:
  [ ---> whitespace ---------------------------- ] -->
     |                                       |
    ,--> value ------------------------------|
    |                                        |
    |________________________________________|
```

and so on, there's also strings, numbers and whitespaces.
async / await execution order

in JS theres a function called an async function:
```js
  async function x(){
    return 1;
  }
```

Many functions are provided by JavaScript host environments that allow you to schedule asynchronous actions, In other words, actions that we initiate now, but they finish later.

for example, there's the setTimeOut function.

let's take a look at it:

```js
  setTimeOut (() => {
    console.log("this message appers after 2 seconds");
  }, 2000);
```

2000 means 2000 milliseconds, which is 2 second. this is basic usage, let's take a look at the syntax:

```js
  setTimeOut(function, delay, param1, param2, ...);
```
this is how we pass the parameters:

```js
  function x(name){
    console.log(`hello, ${name}`);
  }

  setTimeOut(x, 3000, "programmer");
```

x is the function to execute, 3000 is the delay before the function executes,
and "programmer" is the parameter pased to the function.

let's take a look at the function loadScript(src), that loads a script with the given src:

```js
  function loadScript(src){
    let script = document.createElement('script');
    script.src = src;
    document.head.append(script);
  }  
```

we created a <script> tag and append it to the page, this causes the script
with the given src to start loading and run when complete.
