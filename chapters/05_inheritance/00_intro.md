# 05 Inheritance

In classical languages like C++ or Java, objects are instances of classes. Classes are abstract definition of what each instance of that class should look like and an object follows the class' definition, while containing concrete data. In those languages, classes inherit from classes. In JavaScript there are no classes, which is why a classical inheritance model is not applicable. JavaScript makes use of a different concept: Prototypal inheritance.

Most of the time in this chapter, the term "classical" is supposed to mean "class-based", since that describes the inheritance model of languages like C++ and Java. In contrast to those, JavaScript is actually object-based or object-oriented, which makes it stand apart from classical languages.

Along with first-class functions, prototypal inheritance is one of the core concepts of JavaScript. While feeling unfamiliar to most programmers, coming from other (classical) languages, these features make JavaScript extremely flexible, allowing the programmer to choose the paradigms and the style, he prefers.

In this chapter, I will explain how inheritance in JavaScript works, and show a handful of ways to create objects and implement inheritance. Some of the patterns, you will learn in this chapter, are extremely powerful, others are of little use. These are presented to illustrate what is possible, using the tools of the language or maybe even to demonstrate you, what you should not be doing. But maybe even more important is, that all the patterns introduced are meant to give you a better understanding of how the language works and to motivate you to come up with more ideas on how to create objects and structure those object's interplay.