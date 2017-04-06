# alphanum-increment

A small library that increment or decrement an alpha-numeric string

## Installation

  `npm install alphanum-increment`

## Usage

    const alphanuminc = require('alphanum-increment);
    const increment = alphanuminc.increment;
    const decrement = alphanuminc.decrement;

    increment('aa'); // output 'ab'
    decrement('abc'); // output 'abb'

## Options

By default, increment and decrement functions are based on this string :
abcdefghijklmnopqrstuvwxyz0123456789-

##### alpha
If true, all alpha chars (of s_alpha parameter) are included in the base string. Default: true

##### digit
If true, all digit chars (of s_digit parameter) are included in the base string. Default: true

##### dashes
If true, a dashe (hypens) will be included in the base string. Default: true

##### specials
If true, all spacials chars (of s_specials parameter) are included in the base string. Default: false

##### orderby
Define the order of alpha chars and digits char in the base string.
Default: "ALPHADIGIT"
Values: ALPHADIGIT or DIGITALPHA

##### s_alpha
Define the string of alpha chars.
Default: "abcdefghijklmnopqrstuvwxyz"

##### s_digit
Define the string of digits chars.
Default: "0123456789"

##### s_specials
Define the string of specials chars. You must add some specials chars and set the parameter "special" to true if you want to use there's.
Default: ""

## Tests

  `npm test`
