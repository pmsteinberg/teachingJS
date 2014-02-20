## Preface

This is a living document.

### How I approached this book
This book was created as a script for a workshop on JavaScript. I wrote it to gather my knowledge, to put it into words, to structure it, to illustrate it with examples. I assume the reader is familiar with programming in general and I sometimes compare JavaScript to Java, but Java skills are not required. I sometimes also assume a basic knowledge of programming patterns or field specific terms. If you have never been programming before, this might not be a book for you.

I would love this book to be self-explainatory enough for it to be read without attending the related workshop, but as of now it isn't. I want it to be a reference containing all there is to know, but it is not complete yet. I want it to be structured in a way that encapsulates topics in their own self-contained chapters or subchapters and I also want it to read better than a boring reference, but it is not there yet. All of these goals may never be met completely, because it is impossible to cover every edge case of the language and because there will always have to be a compromise between readabilty and correctness or completeness.

So as my work on this book progresses, my understanding of the language will change and even the language itself will change.

### How time approaches this book
By the time of writing (early 2014), the most recent version of the language specification is ECMA262 Edition 5.1 (2011). Sometimes I point out changes frmo Edition 3 and I regularly include explanations on things that are going to be in Edition 6. But when there is no explicit information on the version of the language in which a certain feature exists or not, assume that I am talking about ES5.1. Most likely, you want to write code to be run inside a web browser. Fortunately, ES5 compatibility is more or less present in all current web browsers: Firefox 4+, Chrome 13+, Internet Explorer 10+, Safari 6+. ES6 support is not yet at a level at which you want to rely on ES6 features; give that some more years.

Every few months there is a new version of Firefox and Chrome and it will not take a long time until the notes on ES6 support regarding certain browsers in this book are outdated. In the meantime, the specification process for ES6 is still going on for who knows how long and things might change eventually. But this book is not considered "done": As things change, so will this book (hopefully).

### How you should approach this book
Of course you can read this book however you like, but let me give you some information about how you get the most out of it. In trying to cover a topic in its completeness, I might introduce a level of detail that you find unnecessary. Feel free to skip over anything you are not interested in or what you think is confusing. You can also freely skip over any parts that I labeled more or less explicitly as being optional. You can always come back to those (advanced or just unimportant) paragraphs later and I tried to include a lot of cross-references to let you know where you can read up on a topic. This should motivate you to read just the chapters of the book you are interested in.

That does not mean, that the way in which the chapters and subchapters are ordered is irrelevant.

### How this book approaches this book
After this introduction to the text, there will be a chapter on the history of JavaScript. It may influence your understanding of the language to know where it came from, what its influences are and how it developed over time. The history covers the past, the present and the future.

The introduction to the language itself will start with the fundamentals. First, there will be a short part on how you can execute your own JavaScript code. Then the atoms and molecules of JavaScript are presented, the statements that compose a program, the operators that combine values to new values, the types of data you can manipulate in JavaScript and the weird mechanics of how JavaScript manipulates those data itself.

What follows, is a short primer on objects, explaining what they are and how to work with them. But the real power of objects will be released later in a chapter about inheritance. Inheritance is the way in which objects are related to each other and is a really important thing to talk about.

But inheritance in JavaScript does not work without functions, so we will introduce them before talking about inheritance. Functions are a very important and a very beautiful thing about JavaScript and the chapter that covers them should teach you everything you need to know.

### How others approach their books
A lot of pages have been written on JavaScript and you should probably read some of them. When you search for a book on JavaScript, you will probably stumble upon one of these:

- [Marijn Haverbeke - "Eloquent JavaScript"](http://eloquentjavascript.net/). This book will be especially valuable to people how want to learn JavaScript without any experience or prior knowledge in programming. The book is a quick and straightforward introduction to the language and covers working with the DOM.
- [Cody Lindley - "JavaScript Enlightenment"](http://www.javascriptenlightenment.com/). This is not an introductory book that toys around with basic stuff, nor does it cover every aspect of JavaScript. Its strength lies in an extensive look at objects, constructors and builtin wrapper objects.
- [Douglas Crockford - "JavaScript - The Good Parts"](http://javascript.crockford.com/). What many consider the JavaScript bible offers a balanced level of detail and valueable information on how to leverage the language's full potential. This book teaches you how to write good code and how to avoid dangerous parts of JavaScript.
- [David Herman - "Effective JavaScript"](http://effectivejs.com/). Being targeted at people who already know a bit of JavaScript, this book has a ton of information on weird behavior of the language and edge cases you could have never have thought of. It consists of 68 items that dig into a lot of very concrete and some abstract situations and the advice contained in this book will make you a better JavaScript programmer.