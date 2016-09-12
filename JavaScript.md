# JavaScript RTS investigations

Some notes on languages that compile to JavaScript with regard to writing my RTS.

## Plain JavaScript
I started writing my Real Time Strategy game in plain Javascript.

## ->Babel
Then moved to Babel for more features, but in the end Babel compilation was too slow and the JavaScript too messy.

## ->ClojureScript
Then I moved to ClojureScript and incremental compilation together with figwheel is fast enough, a second or two.
Hot reloading is awesome, but the generated JavaScript is not too pretty. Also library is quite big and there are a 
gazillion small .js files, and reloading the web worker (without figwheel) is quite slow since it's not incremental.
Refactoring is not so easy, because of missing static typing and IDE support.

## Bridge.NET?
I was working on another project in C# and I came to enjoy the productivity of static typing and good IDE support for refactoring.
So now I am looking at Bridge.NET to compile C# to JavaScript. Compilation seems fast enough and it generates pretty JavaScript.
Preliminary testing with [hotswap.js](https://github.com/geo-at-github/hotswap.js) and just deleting the app namespace before 
reload indicates that hot reloading should work fine too.

Bridge.NET compilation seemed fast enough: 5 seconds on a clean build of a small project,
it's a bit much actually now that I timed it.
However, coming from ClojureScript, F# might be nicer and with less type declarations.

## Fable or WebSharper?
For F# there are two big projects that compile to JS, Fable and WebSharper.
However, Fable uses Babel and indeed, compiling an empty project took 10 seconds.
WebSharper 4 beta also takes a good while to compile the template project, 12.75 seconds.
WebSharper also brings some library weight and generated JavaScript is not so pretty.

## TypeScript?
TypeScript does have the static typing and IDE support, but feels much less attractive than C# or F#.
I haven't tested compilation time yet.

## Sweet.js?
I don't know if it's fast enough and it does not bring static typing or IDE support, but does bring power of macros. However,
might stick with ClojureScript over this one until it supports static typing.

## NemerleWeb?
Does have both static typing and macros, but IDE support is poor (stopped working when I was testing macros).
I don't remember if I checked compilation time.

## Conclusion
What brings the greatest productivity?
Should I trade off longer compilation time for static typing and IDE support?
Both C# and F# have compiler API, so it is possible to bolt on something like macros if I need it.
Or should I go back to plain JavaScript to avoid compilation time and use more rigorous components with functional programming?
Maybe I will investigate ClojureScript IDE support with Cursive and stick with it.
