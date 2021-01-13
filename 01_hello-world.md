Python 3 and VSCode are assumed to be already installed on your machine.

Let's start with the traditional `hello world` program.

This is a simple program that instructs the computer to say (actually print) "Hello, world!".

## Program

First, create a new directory (folder) and name it `hello-world` (or whatever name you like).

Open the directory in VSCode.

Create a new file in the directory and name it `hello_world.py`, then write in the following:

```python
print("Hello, world!")
```

Save, and finally open the terminal and run the following command:

```shell
python hello_world.py
```

If you're on macOS, replace `python` in this command with `python3`. 

This command will execute the program.

Alternatively, you can click on the run button on the top right corner of the window.

If everything goes right, you will get the output:

```output
Hello, world!
```

## Analysis

Now, let's break things down.

The program is made of one line of code.

This one line is made of two parts:

1. A **function** named `print`
2. A **string** with the value `"Hello, world!"`

The following is a brief overview of what functions and strings are, just to understand what this program really is. We will talk about them in detail later.

### Function

A function is identified by a **name**, it takes in an **input** and produces an **output**.

In our program, the name is `print`, which is a builtin function in Python, the input is the string `"Hello, world!"` and the output is printing the same string `"Hello, world!"` on the terminal.

To **call a function** (have it do what it does), we write its name, followed by parentheses, and inside the parentheses we write the input.

So like this:

```python
my_function(my_input)
```

If we omit the parentheses, we get an error:

```python
print "Hello, world!"
```

```output
SyntaxError: Missing parentheses in call to 'print'. Did you mean print("Hello, world!")?
```

### String

A string is one of several **data types** in Python and it is used to store _text_.

Text here means any sequences of [valid characters](https://en.wikipedia.org/wiki/List_of_Unicode_characters) (#, %, a, 8, ~, ∂ ...).

A string must begin and end with either single quotes (`'`) or double quotes (`"`).

The opening and closing quotes are not part of the text's value, they are just an indicator to instruct Python where to start and where to stop scanning the text.

There is another way of representing strings which we'll see later.

Here are a few examples of valid and invalid strings:

- Valid:
  - `"hello"`
  - `'hello'`
  - `"¡™£™££¢"`
- Invalid:
  - `hello`
  - `"hello'`

Let's test the invalid ones:

```python
print(hello)
```

```output
NameError: name 'hello' is not defined
```

`hello` is treated as a name, and since you haven't defined what this name should refer to in the program you get this `NameError`.

```python
print("hello')
```

```output
SyntaxError: EOL while scanning string literal
```

Python encountered an opening double quote and started scanning a string, but it did not stop at the single quote (because that's not meant to be), it kept going and reached the end of the line (EOL) without completing the scan of the string. And this is a `SyntaxError` error.