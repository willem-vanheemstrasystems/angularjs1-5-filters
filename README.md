# angularjs1-5-filters
AngularJS 1.5 Filters

Based on 'AngularJS filters' at https://www.youtube.com/watch?v=Y2Few_nkze0&list=PL6n9fhu94yhWKHkcL7RJmmXyxkuFB3KSl&index=8

#Filters in AngularJS

Filters in AngularJS can do three different things:

1. Format data
2. Sort data
3. Filter data

Filters can be used with a binding expression or a directive.

To apply a filter, use the pipe (|) character

```javascript
{{ expression | filterName:parameter }}
```

#Filters for formatting data

Filter      : Description
***lowercase***   : Formats all characters to lowercase
***uppercase***   : Formats all characters to uppercase
***number***      : Formats a number as text. Includes comma as thousands separator and the number of places can be specified 
***currency***    : Formats a number as a currency. $ is default. Custom currency and decimal places can be specified
***date***        : Formats date to a string based on the requested format

##Angular Date Formats

Format      : Result
***yyyy***  : 4 digit year, example 1998
***yy***    : 2 digit year. example 1998->98
***MMMM***  : January-December
***MMM***   : Jan-Dec
***MM***    : 01-12
***M***     : 1-12 (No leading zeros)
***dd***    : 01-31
***d***     : 1-31 (No leading zeros)

See the official documentation at https://docs.angularjs.org/api/ng/filter/date

The ```limitTo``` filter can be used to limit the number of rows or characters in a string.

```javascript
{{ expression | limitTo : limit : begin }}
```

See script.js and index.html to see how to apply filters.