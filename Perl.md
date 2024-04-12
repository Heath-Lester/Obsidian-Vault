https://www.tutorialspoint.com/perl/perl_data_types.htm

<iframe width="100%" src="https://www.youtube-nocookie.com/embed/74_7LrRe5DI?si=nrHAEivdPTJfLF1v" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen style="border-radius: 4px; aspect-ratio: 16/9;"></iframe>
 
## EYNTK about Perl
- Developed in 1987
- latest version is 5
- cross platform language
- version 6 became another language called Raku
- loosely typed language ([[Loosely vs Strongly Typed]])
- interpreted language ([[Interpreted vs Compiled Languages]])
- dynamic typed language ([[Dynamic vs Static Typed]])
- scripting language ([[Scripting vs Programming Language]])
- known for powerful text processing abilities
- Is called a glue language
- Commonly used to write CGI scripts ([[Common Gateway Interface]])
- Used by high traffic sites like DuckDuckGo, Booking.com, and Craigslist
- Syntactically resembles C
- Syntax can be very compressed
- Contains a lot of primitive types
- variables are declared with a `$` prefix
- `$` variables are called scalars, meaning they only contain a single value
- uses `my` and `our` as access specifiers to be `private` and `public` respectively ([[Access Specifiers]])
- arrays are declared with the `@` prefix
- uses bracket `[]` access with index for arrays
- hashes are declared with the `%` prefix
- uses brace `{}` access with key for hashes
- conditional statements use `if` , `elsif` and `unless`
- can use the ternary `?` operator
- functions are called subroutines and defined as `sub name {}`
- parameters are defined inside the logic of subroutines using `@_`:

```perl
sub PerWillBeFunTheySaid {
	print "this is a function\n";
	my ($n1, $n2) = @_;

	print $n1 + $n2;
}
```

- Regex is built into Perl which comes with a binding operator `=~` that allows a string to be matched with a regular expression
- Comes with autovivification which will create all the elements in an array which do not yet exists if the value at an index that does not exists in an array is incremented 


### Data Types

| Sr.No. | Types & Description                                                                                                                                                                                                                          |
| ------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1      | **Scalar**<br><br>Scalars are simple variables. They are preceded by a dollar sign ($). A scalar is either a number, a string, or a reference. A reference is actually an address of a variable, which we will see in the upcoming chapters. |
| 2      | **Arrays**<br><br>Arrays are ordered lists of scalars that you access with a numeric index, which starts with 0. They are preceded by an "at" sign (@).                                                                                      |
| 3      | **Hashes**<br><br>Hashes are unordered sets of key/value pairs that you access using the keys as subscripts. They are preceded by a percent sign (%).                                                                                        |

#### Numeric Literals

| Type                | Value    |
| ------------------- | -------- |
| Integer             | 1234     |
| Negative integer    | -100     |
| Floating point      | 2000     |
| Scientific notation | 16.12E14 |
| Hexadecimal         | 0xffff   |
| Octal               | 0577     |

#### String Literals

|Escape sequence|Meaning|
|---|---|
|\\|Backslash|
|\'|Single quote|
|\"|Double quote|
|\a|Alert or bell|
|\b|Backspace|
|\f|Form feed|
|\n|Newline|
|\r|Carriage return|
|\t|Horizontal tab|
|\v|Vertical tab|
|\0nn|Creates Octal formatted numbers|
|\xnn|Creates Hexideciamal formatted numbers|
|\cX|Controls characters, x may be any character|
|\u|Forces next character to uppercase|
|\l|Forces next character to lowercase|
|\U|Forces all following characters to uppercase|
|\L|Forces all following characters to lowercase|
|\Q|Backslash all following non-alphanumeric characters|
|\E|End \U, \L, or \Q|