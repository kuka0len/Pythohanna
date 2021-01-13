## A bit of theory

>All programming is processing of data.

And variables are what we use to store and refer to data.

A variable has a **name** and a **value**. It actually has other properties which we'll talk about later, but now let's focus on these two.

### Name

A variable name is an identifier that is used to uniquely refer to some data.

Rather than directly using the data where it's needed in the program (which can be impractical and almost-impossible), we use its significantly shorter name instead.

Names also help give meaning to our data, and it is extremely important to give good and meaningful names to our variables.

Without naming data, it is practically impossible to do any programming.

A valid Python variable name has to obey the following:

- Can only contain letters (`a`-`z`, `A`-`Z`), numbers (`0`-`9`) or underscores (`_`)
- Must start with a letter (`a`-`z`, `A`-`Z`) or underscore (`_`)

Here are a few examples of valid and invalid variable names:

- Valid:
  - `x0`
  - `hello`
  - `_error`
- Invalid:
  - `0_people`
  - `x-1`
  - `perkeläinen`

Note also that variable names are case-sensitive, so `user1` and `User1` are not the same thing.

### Value

The value of a variable can be any valid Python data.

An example of data we've already seen is a string, e.g. `"Well, excuse me, princess!"`.

We'll talk more about data later.

### Defining a variable

To define a variable we have a very simple syntax: we write the name, followed by an equal sign (`=`), also called the **assignment operator**, and finally followed by the value.

Example:

```python
my_name = "Johanna"
```

## Practice

Now let's rewrite the `hello world` program and use a variable as input instead of directly using the data:

```python
hello = "Hello, world!"
print(hello)
```

```output
Hello, world!
```

Works as expected.