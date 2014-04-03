0x24
====

The dollar sign or 0x24, its UTF-8 (hexadecimal) specification, has a long history of use throughout various computer programming languages. It is commonly used as a utility class in JavaScript, where it defines a set of functions that perform common and often used actions. Here, it is used as a prefix for the 0x24 JavaScript live templates, frequently used snippets of code, developed for use with [WebStorm](http://www.jetbrains.com/webstorm/).

Naming Conventions
------------------

### Basic

A live template name is prefixed with a dollar sign and a unique identifier derived from the framework where it originates from (e.g. Jasmine live templates use $j as a prefix). The next sequence of letters in a live template name are derived from the name(s) of the function(s) included in the live template (e.g. the beforeEach function uses the letters 'be'). The complete live template name for a Jasmine beforeEach function is $jbe.

### Collisions

Live templates where basic naming conventions result in a duplicate name include additional sequential letters of the last function name until a unique name is determined (e.g. Angular live template names for the filter and factory functions respectively are $ngfi and $ngfa).

### Combining

Live templates that include functions from multiple frameworks begin with the naming convention used for the primary template set followed by the naming convention for the secondary set, omitting the dollar sign for the secondary set (e.g. the live template name for a Jasmine beforeEach function with an Angular inject function is $jbengi).

Samples
------

### Jasmine

`$jd` ((j)asmine (d)escribe)

```JavaScript
describe('$foo$', function() {
    $END$
});
```

### Angular

`$ngsw` (a(ng)ular (s)cope (w)atch)

```JavaScript
$scope.$watch('$foo$', function(newValue, oldValue) {
    $END$
});
```

### Node

`$nrcr` ((n)ode (r)equire (cr)ypto)

```JavaScript
var crypto = require('crypto');
$END$
```

*The 0x24 live templates use the enter key for expansion.*

Installation
------------

Save the 0x24.xml file to one of the following locations depending on operating system:

+ Windows: [home directory]\.[product name][version number]\config\templates
+ Linux: ~\.[product name][version number]\config\templates
+ MacOS: ~/Library/Preferences/[product name][version number]/templates

*The live templates will be available for use after the next restart of the IDE.*
