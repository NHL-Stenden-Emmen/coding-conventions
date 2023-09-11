# Coding Conventions
Meet the standards for Informatica and Information Technology

## Naming

- Use meaningful names
Use descriptive names for all identifiers (names of classes, variables and methods. Avoid ambiguity. Avoid abbreviations.
Simple mutator methods should be named `setSomething(...)`.
Simple accessor methods should be named `getSomething(...)`.
Accessor methods with Boolean return values are often called `isSomething(...)`, for example `isEmpty()`.	

- Class names start with a capital letter.

```java
class Post
```

- Class names are singular nouns.

- Methods and variable names start with lowercase letters.
All the – class, method and variable names – use capital letters in the middle to increase readability of compound identifiers, e.g. `numberOfItems`, also called `lowerCamelCase`.

- Constants are written in UPPERCASE.
Constants occasionally use underscores to indicate compound identifiers (SCREAMING_SNAKE_CASE): 
`MAXIMUM_SIZE`

- Suffix exceptions with `Exception`.

```java
class MyOwnException
```

- When calling methods or fields from the current class, **always** prefix them with `.this`.

```java
this.firstName

this.doSomething()
```

### (Unit) Testing

- For methods of Unit Tests we use the following convention:

```java
void methodThatIsBeingTested_expectedValue_howIsTested()
```

## Layout

- One level of indentation is four spaces.

- All statements within a block are indented one level. 
- The braces for class method and structural blocks are on separate lines and are at the same indentation level, for example:

```java
public int getAge()
{
    statements
}

while (condition)
{
    statements
}


if (condition)
{
    statements
}
else
{
    statements
}
```

- Always use curly brackets in control structures. Curly brackets are used in if-statements and loops even if the body is only a single statement.

- Use a space around operators (=, +, -, *, %, /).

```java
int sum = 5 + 6;
double multiple = 5 * 6;
```

- Don’t use a space between the method name and the opening parenthesis of the parameters.

- Use a space between the parameters of a method, so after each comma.

```java
public void method(int param1, int param2)
```

- Use a space between (operational) keywords like `if, while, for` and the opening parenthesis.

```java
while (condition)
if (condition)
for (condition)
```

- Don’t use a space for incrementing and decrementing operators, for example:

```java
number++;
```

- Use a blank line between methods (and constructors). Use blank lines to separate logical blocks of code. This means at least between methods, but also between logical parts within a method.

```java
public int method()
{
    return 1;
}

public int anotherMethod()
{
    return 2;
}
```

- Add a blank line before a return statement.

```java
public void method()
{
    statements
    statements

    return;
}
```

- Fields should be declared in the top of the class, before constructor(s) and methods.

```java
class MyClass
{
    Fields

    Constructor

    Getters and setters

    Methods
}
```

- Getters and setters should be bundled. So, for example, if we have two fields `name` and `number` we would have:

```java
public String getName()
{
}

public void setName(String name)
{
}

public int getNumber()
{
}

public void setNumber(int number)
{
}
```

- Custom methods should be placed below getters and setters.

## HTML & CSS

- Don't use whitelines in your HTML.

- Every nested tag should be indented.

- Tags should be in lowercase.

```html
<button></button>
```

- Don't use spaces around `=` signs.

```html
<img src="image.png" alt="A black and white cat" />
```

- Use lowercase for your filenames.

```
index.html
about-us.html
style.css
```

- Don't place a space after opening a tag paragraph tag.

```html
<p>I don't need a space</p>
```