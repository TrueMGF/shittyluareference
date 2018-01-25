# Operators 
## TL;DR

- Arithmetics: `+`, `-`, `*`, `/`, `%`(Modulo), `^` (x to the power of y), 
- `>` (greater) and `<` (less), `>=` (greater or equal to), `<=` (less or equal to), `==` equals, `~=` does NOT equal
- `and`, `or`, `not` represent the concept of their same name

## if Niko\_is\_bowling == false then go\_bowling()  
Sometimes, you want code to only run under certain circumstances. We use Operators and conditional structure for these.

Operators are anything comparing two values, whilst conditional code only runs if it's condition is fulfilled - usually checked with those operators. We'll cover conditional code in the next page.

### Operators
Every operator will compare the value to it's left to the value on it's right.

We already know about comparing two values exactly to each other from earlier: `==` and `~=`.

The first operator `==` returns `true` if both values are exactly the same. This also means that if the datatype does not match, the comparison will return false!

The second operator with the squiggly line, `~=` does the exact opposite. If the values DON'T match, it returns true.

```lua
print("hello" == "hello") --returns true
print(42 == "42") --returns false - datatypes don't match! No coercion here.

print(69 ~= 420) --returns true - because the values don't match.
let ayylmao = "ayylmao"
print(ayylmao ~= "ayylmao") --returns false - the variable content is identical to the compared value!
```

Time for some MATH. You love that, don't you?

There are four operators that let you compare your variables in size: `<`, `>`, `<=` and `>=`. All of them should be really self explanatory:

`<` will return `true` if the left value is smaller than the right value. Adding the equals sign (`<=`) will return `true` if the left value is smaller *or equal to* the right value.

On the contrary, `>` will return `true` if the left value is greater than the right value, and the added equals sign (`>=`) will also return `true` if the left value is greater or equal to the right value.

Confused? In school, I was always taught it like this: Think of the comparison signs as a crocodiles (or an alligators) snout. The crocodile wants to eat stuff, but it will only eat stuff it can actually swallow - stuff smaller than itself.  You won't see a crocodile eating an elephant... right?

Now here's something interesting - this also works on alphabetical sorting. A is the "smallest" and Z is the "biggest"!

```lua
small = 69
big = 420
print(small < big) --true
print(small > big) --false
print("aaa" < "abc") --true
print("remove kebab") --remove kebab   Just remove it from the premises already 
```

### Logical Operators
Now for the logical operators. There are three flavours of these: `and`, `or`, and `not`.

`not` will invert the result you get, turning a true into a false and vice versa.

`and` requires both the first statement and the following statement to be true so that itself can output true.

`or` only requires one of the statements to be true, but doesn't mind if both were, either.

```lua
print(not true) --false, duh.

print(true and true) --true
print(true and false) --false

print(false or false) --false
print(false or true) --true
print(not true or true) --you can mix and match this stuff, try not to confuse yourself with not though.
``` 
