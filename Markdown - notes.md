## Table of contents

* [Headers](#headers-up)
* [Text formatting](#text-formatting-up)
* [Links](#links-up)
* [Images](#images-up)
* [Lists](#lists-up)
* [Tables](#tables-up)
* [Code and Syntax highlighting](#code-and-syntax-highlighting-up)
* [Blockquotes](#blockquotes-up)
* [Line breaks](#line-breaks-up)
* [HTML styling](#html-styling-up)


## Headers [(up)](#table-of-contents)

```
# Header 1
## Header 2
......
###### Header 6
```
# Header 1
## Header 2
**......**
###### Header 6


## Text formatting [(up)](#table-of-contents)

```
*Italic*
**Bold**
***Bold and italic***
~~Strikethrough~~

Alternatively, __underscores__ can be used or **_combined_** with asterisks.
```
*Italic*<br>
**Bold**<br>
***Bold and italic***<br>
Alternatively, __underscores__ can be used or **_combined_** with asterisks.


## Links [(up)](#table-of-contents)

```
[Link](http://www.example.net/)
[Link to a header](#header-name)
[Link to a repository file](./README.md)
```
[Link](http://www.example.net/)<br>
[Link to a header](#header-name)<br>
[Link to a repository file](./README.md)


## Images [(up)](#table-of-contents)

```
![alternative text](http://www.w3schools.com/html/html5.gif "Title")
```
![alternative text](http://www.w3schools.com/html/html5.gif "Title")

"Title" is optional and the brackets can be left empty.


## Lists [(up)](#table-of-contents)

Creating unordered list can be done with `*`, `-`, or `+`.<br>
Ordered lists are created by using numbers.
```
1. First ordered list item
2. Second ordered list item

* First unordered list item
+ Second
- Third
```
1. First ordered list item
2. Second ordered list item

* First unordered list item
+ Second
- Third


## Tables [(up)](#table-of-contents)

Table columns are separated by pipes (`|`).<br>
First row contains the headers. Second row has to have at least 3 dashes (`---`) for each column.<br>
Colons (`:`) are used on the second row for alignment (default is left).
```
Left alignment | Centered | Right
-------------- | :------: | ----:
*row 3*        |    `1`   |   2
__row 4__      |     3    |   4
```
Left alignment | Centered | Right
-------------- | :------: | ----:
*row 3*        |    `1`   |   2
__row 4__      |     3    |   4


## Code and Syntax highlighting [(up)](#table-of-contents)

Inline code has one back-tick around it.<br>
Multiline code is surrounded by three back-ticks. (example uses 2 because they can't be nested...)
```
This `is inline` code.

``
Multi
    Line
        Code
``
```

This `is inline` code.

```
Multi
    Line
        Code
```

Syntax highlighting:
```
``java
public class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hello, World");
    }

}
``
```

```java
public class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hello, World");
    }

}
```

### Common supported language syntaxes

Language | ```alias
-------- | :------:
BASH | `sh, bash`
C | `c`
C++ | `cpp, c++`
C# | `csharp`
CSS | `css`
Clojure | `cj, clojure`
Dart | `dart`
Go | `go`
Groovy | `groovy`
HTML | `html`
Java | `java`
JavaScript | `js, javascript`
JSON | `json`
Haskell | `hs, haskell`
Matlab | `matlab`
MySQL | `mysql`
Objective-C | `objc`
PHP | `php`
PowerShell | `posh, powershell`
Python     | `py, python`
R | `rout, rconsole`
Ruby | `rb, ruby`
Sass | `sass`
SQL | `sql`
TeX, LaTeX | `tex, latex`
XML | `xml`

**[A more detailed list of languages](http://tinker.kotaweaver.com/blog/?p=152)**


## Blockquotes [(up)](#table-of-contents)

```
> This

> is a

> blockquote.

```
> This

> is a

> blockquote.


## Line breaks [(up)](#table-of-contents)

```html
Paragraphs are separated with an empty line between them.

To get text on the following line use the HTML `<br>` tag. <br>
Like this.
Otherwise, text gets typed on the same line.
<br> <br> <br>
Use more `<br>` tags for more than one line between paragraphs.
```

Paragraphs are separated with an empty line between them.

To get text on the following line use the HTML `<br>` tag. <br>
Like this.
Otherwise, text gets typed on the same line.
<br> <br> <br>
Use more `<br>` tags for more than one line between paragraphs.


## HTML styling [(up)](#table-of-contents)

```html
<style>
    .example {
        border: 2px solid green;
        border-radius: 10px;
        padding: 5px;
        text-align: center;
    }
</style>

<p style="color: cyan">Traditional HTML can be used to write Markdown.</p>
<p class="example"> Applying styles with the <em>`<style>`</em> attribute or tag.</p>
```
**Due to security reasons (most probably) GitHub prevents CSS from rendering, but Markdown supports it.**
