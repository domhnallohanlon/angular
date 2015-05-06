# Getting started with Angular

a simple, responsive app using angular and bootstrap.



## Directives

Directive are angular-specific attributes which are added to HTML tags to run or reference some JavaScript code.

A directive typically starts with the prefix `ng-`

### More directives

Directive       | Usage
----------------|------------
`ng-app`        | attaches the application module to a page, via the `<html>` tag
`ng-controller` | attach a controller function to a page, typically in the `<body>` or some other container
`ng-show`       | show an element based on a boolean expression
`ng-hide`       | hide an element based on a boolean expression
`ng-repeat`     | repeat an element, or section of elements, for each item in an array.
`ng-src`        | for specifiying the source of a file/image


## Modules

Individual pieces of an application are modules. This modular approach makes code more maintainable and easier to test. 

Modules can also include dependencies 


## Expressions

Expressions allow you to insert dynamic values into static HTML pages. You can recognise them by their double curly braces `{{ }}`

## Controllers

A controller is a piece of JavaScript that defines the functions and values available to your app. 

Best practice is the wrap your JavaScript in a closure and to use the word 'Controller' in the name of 

### Scope

It is worth pointing out that the scope of a controller is limited to the DOM element that references it.

## DRY programming

Don't repeat yourself...let the code do that for you.

##Filters

Filter are denoted by pipes - just like grep etc. - so you send the output of the data into the filter.
Typical syntax:
`{{data | filter:options}}`

### Useful Filters

`value | currency : "symbol" ` display a number as a dollar amount. The symbol option allows you to pass an alterantive currency symbol, e.g. "£" or "€".

`date : fo/rm/at` convert a unix time to whatever format you like. `M` is used for month since `m` represents minutes

`uppercase` & `lowercase` does what it says on the tin

`limitTo : ammount` takes and integer argument and uses that as a stopping point

`orderBy: 'value'` order from smallest to largest value
`orderBy: '-value'` order from largest to smallest value 