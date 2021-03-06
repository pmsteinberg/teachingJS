## The Metamorphosis and the Struggle (2000-2011)

Besides the official standardization efforts, there were at least two other major processes that changeed the course of the language's history.
.
### Ajax
Browsers implemented an API to make HTTP requests in JavaScript which was a feature that was underestimated at first. Until 2005 when Interaction Designer Jesse James Garrett and his company, Adaptive Path, were experimenting on how to improve user experience when browsing a website. In order to improve performance and responsiveness, Garrett came up with the idea, that instead of doing full page replacements, he could use the HTTP interface to only fetch the part of the page that needed to be replaced, when a new page was requested. Because things like navigations and side bars often stay the same across one website it is unnecessary to send those pieces of HTML over the wire everytime a user wants to visit a new page. The new technique resulted in smaller files and thus shorter loading times. For this new concept, Garrett coined the term *"Asynchronous JavaScript and XML" (AJAX)*.

Not only made Adaptive Path their clients happy, but they also started a *Metamorphosis of JavaScript*. The language had gained traction over the years because it was the only programming language for the web and if you wanted to build some kind of interaction into your site you would have to use JavaScript or Flash. The later has a higher level of entry for programmers, but JavaScript was easy to use, forgiving and just enough to create animations like dropdown menus and that sort of things. But along with the AJAX revolution, developers started to realize that it was possible to build complex applications in JavaScript. Ajax made it possible to load separate parts of an application one by one and only if needed so the user would not have to wait for a lot of application code to be downloaded and initialized.

One of the important aspects of Ajax is the keyword "asynchronous": Browsers are generally single-threaded and the browser UI runs in the same thread as the JavaScript code. So when a computation in JavaScript takes a long time, the browser UI would not respond to user activity until JavaScript is finished running. Now this means that when an HTTP request would take some time to get a response from the server, the UI would be unresponsive which results in very poor user experience. An "asynchronous" HTTP call circumvents this issue by immediately returning and allowing the JavaScript execution and UI to continue. When the server response is received a callback function is invoked, reacting to the received data. This pattern introduces more complexity to an application but greatly improves user experience.

### ES4
Back to the standardization process. While first proposals on the next language edition were made as of 1999, the commitee was torn on how big a change to implement in the new version. There were two factions, one of them promoting concepts with a lot of new syntax and semantics, while the other part of the committee favored small and careful adjustments over the introduction of revolving features. After a successful meeting in Oslo in 2008 Brendan Eich declared a *"harmony"* among the commitee which became the working title for the next version of ECMAScript. It was decided to quickly agree on a moderate ES3.1, which carefully made minor adjustments to the language. ES4 should then be a greater step forward incorporating concepts like classes, block scope, constants and destructuring. As a diplomatic measure, ES3.1 was renamed to ES5 and ES4 was renamed to ES6; the problematic fourth edition was left out.

The struggle was overcome and ECMAScript 5th Edition was published in 2009. Some more changes accumulated and were addressed in another minor specification version as ES5.1 in 2011 making this the current version of the language.

### Strict Mode
ES5 also includes what is called the *"Strict Mode"*. Strict mode defines a subset of JavaScript that disallows some of the potentially harmful features. If you don't understand the following list, don't be afraid: You probably will, after reading this book. Strict mode adds a handful of `SyntaxError`s that get thrown when you do weird stuff with `eval` and `arguments`. It forbids the use of `arguments.callee` and `arguments.caller`, octal number literals, `with` and it makes the default binding of `this` be `undefined` instead of the global object.

How to enable Strict Mode? You simply have to include a string as the first statement in your function. That makes this function and all functions defined within it be executed in strict mode.
```javascript
(function () {
    'use strict';

    // ... your application code

}());
```
There is also a file-wide form of strict mode, where `use strict;` is the first statement in your code.

Strict Mode is supported by Firefox 4+, Chrome 13+, Internet Explorer 10+ and Safari 6+. These browsers will recognize the `'use strict';` statement and treat your code as strict code. Environments that do not support Strict Mode will simply ignore the `'use strict';` statement because it is a regular string expression with no effect. There is also a function form for Strict Mode: You include the `'use strict';` statement as the first statement in a function body and then this function will be executed in strict mode. It is generally not possible to toggle browser consoles into Strict Mode.

Future versions of the JavaScript language extend on ES5.1 Strict Mode so I advise you to use Strict Mode whenever possible.