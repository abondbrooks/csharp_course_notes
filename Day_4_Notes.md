# C# Notes

### Operators
An **operator** is a set of one or more characters used for calculations.

**Operators** transform one or more data values, known as operands, into new values.

**Example:**

```csharp
x + y
```

**Where:**

x and y are operands
+ is an **operator.**

### Operators in C#:
---


### Arithmetic operators:

| Operator | Description               | Example         |
| -------- | ------------------------- | --------------- |
| `+`      | Addition                  | `x + y`         |
| `-`      | Subtraction               | `x - y`         |
| `*`      | Multiplication            | `x * y`         |
| `/`      | Division                  | `x / y`         |
| `%`      | Modulo (Remainder)        | `x % y`         |

### Arithmetic Assignment operators:

| Operator | Description                      | Example           |
| -------- | -------------------------------- | ----------------- |
| `+=`     | Add and Assign                   | `x += y`          |
| `-=`     | Subtract and Assign              | `x -= y`          |
| `*=`     | Multiply and Assign              | `x *= y`          |
| `/=`     | Divide and Assign                | `x /= y`          |
| `%=`     | Modulo and Assign                | `x %= y`          |

### Relational Operators:

| Operator | Description                   | Example         |
| -------- | ----------------------------- | --------------- |
| `>`      | Greater than                  | `x > y`         |
| `<`      | Less than                     | `x < y`         |
| `>=`     | Greater than or equal to      | `x >= y`        |
| `<=`     | Less than or equal to         | `x <= y`        |
| `==`     | Equal to                      | `x == y`        |
| `!=`     | Not equal to                  | `x != y`        |

### Logical operators:

| Operator | Description                          | Example              |
| -------- | ------------------------------------ | -------------------- |
| `&&`     | Logical AND (returns true if both operands are true) | `x && y`             |
| `||`     | Logical OR (returns true if at least one operand is true) | `x || y`             |
| `!`      | Logical NOT (reverses the boolean value of the operand) | `!x`                 |
| `^`      | Logical XOR (returns true if only one operand is true, but not both) | `x ^ y`              |

### Unary operators:

Unary operators are used on a single operand, and they modify the operand in some way.

#### Increment and Decrement:

```csharp
int x = 5;
x++; // Increment x by 1 (x is now 6)
x--; // Decrement x by 1 (x is now 5 again)
```

Remember to properly use these operators based on your program's requirements and the desired outcomes.