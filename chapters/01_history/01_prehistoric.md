## Prehistoric Events (early 60s to late 80s)

It's hard to tell, where the story ultimately begins. Maybe we would have to go back to the origins of mathematics thousands of years ago. But in order to limit our retrospective to more direct influences on the JavaScript programming language, we will look at two lines of action that brought significant features to the language.

Norway 1967. At the Norway Computing Center Ole-Johan Dahl and Kristen Nygaard created what was the very first object oriented programming language: *Simula*. Simula greatly influenced the design of Stroustrup's C++ and thus basically every object oriented programming language to this day.

### The Great-Grandfathers
But Even older than Simula is another very influencial language. John McCarthy created *Lisp* at MIT in 1958 making it one the first high-level programming languages. It introduced important concepts like higher-order functions and recursion. Lisp is based on the lambda calculus, a turing-complete computational model based on variable binding and substitution. All functional languages and functional features in other languages are strongly influenced by Lisp.

Another one of the great-grandfathers of JavaScript may be Alan Kay. Together with Dan Ingalls he worked at Xerox PARC in the 70s when they created a programming language called *Smalltalk*. The language took the concept of classes and class inheritance from Simula and combined that with an Actor Model implementation. This kind of message passing is today found in web browsers that implement an event firing system for documents. Smalltalk was hugely influencial and was the language in which many object oriented design patterns (like MVC) were implemented for the first time. Smalltalk later also came with a sophisticated development environment that can be seen as the prototype for all modern IDEs. While in JavaScript functions are objects, which is sometimes confusing for newcomers, in Smalltalk basically everything is an object, including code blocks, primitives and even classes.

### The Grandfathers
One of the two most important dialects of Lisp is *Scheme*, which was created by Guy Steele and Gerald Sussman in 1973. Scheme incorporates the Actor Model, uses lexical scoping and was syntactically very close to resembling lambda expressions. Scheme may always have been the little, minimalist, academic brother to Common Lisp, but it was used as the example language in SICP, which made it not only known to computer scientists in general but also to the inventor of JavaScript.

Then there is *Self*. Self was developed by David Ungar and Randall Smith. They also worked at Xerox PARC and as Smalltalk-80 increasingly gained traction in the industry, Ungar and Smith started Self as an experiment to eliminate classes. When applications that were written in Smalltalk grew in size, it became harder and harder to change the most fundamental classes of a program's inheritance hierarchy because that tended to break a lot of subclasses. In Self there are no longer classes, just objects. And these can directly inherit from one another. This approach of cloning one object and modifying it to create a new object is called Prototype-based programming and the inheritance model is called Prototypal Inheritance. This model is also present in JavaScript.