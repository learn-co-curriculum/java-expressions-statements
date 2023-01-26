# Expressions and Statements

## Learning Goals

- Reiterate the difference between an expression and a statement.
- Look at some examples of expressions and the data type they evaluate to.

## Expressions vs. Statements

As we saw in the last lesson, an **expression** is a combination of operators
and variables that evaluate to a single value that has a data type. An example
of an expression is "5 + 2" or "3 < 1". These mathematical expressions describe
a value. In this case, 5 + 2 describes 7 and 3 < 1 describes false.

A **statement** in Java describes activities in a program. For example,
declaring a variable and making an assignment to a variable is an example of a
statement. If we take the mathematical expressions above and assign them to a
variable, then it becomes a statement:

```java
// These are statements
int x = 5 + 2;
boolean a = 3 < 1;
```

Statements, as we have seen, live in a code block. Like the `main()` method that
we have been working with thus far!

```java
public class Main {
    public static void main(String[] args) {
        // This is a code block with statements
        int x = 5 + 2;
        boolean a = 3 < 1;
    }
}
```

## Closer Look at Expressions

Let's take a look at some expressions and the data types they may evaluate to:

| Expression       | Data Type | Result | Explanation                                                                                                                                                                            |
|------------------|-----------|--------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `8 + 4`          | `int`     | 12     | Since 8 and 4 are both integers and the data type is `int`, we can expect 12 to be the result.                                                                                         |
| `7 / 4`          | `int`     | 1      | As we saw in the last lesson, Java will perform integer division when the expression has two `int` as operands, resulting in an `int`                                                  |
| `7.0 / 4`        | `double`  | 1.75   | If one or both of the operands is a `double` when performing division, then real division will occur, resulting in a `double`                                                          |
| `8 == 4`         | `boolean` | false  | Relational operands, like `==`, will result in a `boolean`. In this case, false                                                                                                        |
| `8 != 4`         | `boolean` | true   | Relational operands, like `!=` will result in a `boolean`. In this case, true                                                                                                          |
| `8 * 10 + 4 * 2` | `int`     | 88     | Expressions consisting of multiple operands and operators will still evaluate to a data type. In this case, all operands are integers, so the expression will evaluate to an `int`, 88 |

Your turn! Consider the following variables and see if you can answer the
questions below:

```java
int a = 1;
int b = 2;
int c = 3;
int d = 4;
```

<details>
  <summary>Given the expression, <code>c <= c</code>, what would the appropriate data type be? What is the result?</summary>

  <p>Answer:<br><code>boolean</code> - The expression would evaluate to a <code>true</code>.</p>

  <p><code>c</code> is assigned to the value of 3; and 3 <= 3 is true.</p>

</details>

<details>
  <summary>Given the expression, <code>d % b</code>, what would the appropriate data type be? What is the result?</summary>

  <p>Answer:<br><code>int</code> - The expression would evaluate to a <code>0</code>.</p>

  <p><code>d</code> is assigned to the value of 4 and <code>b</code> is assigned to the value of 2; and 4 % 2 is 0 since 2 goes into 4 an even number of times.</p>

</details>

<details>
  <summary>Given the expression, <code>9.0 / c</code>, what would the appropriate data type be? What is the result?</summary>

  <p>Answer:<br><code>double</code> - The expression would evaluate to a <code>3.0</code>.</p>

  <p><code>c</code> is assigned to the value of 3; and 9.0 / 3 is 3.0. The data type here needs to be a <code>double</code> since the operand, 9.0, is a <code>double</code>.</p>

</details>

<details>
  <summary>Given the expression, <code>a / b</code>, what would the appropriate data type be? What is the result?</summary>

  <p>Answer:<br><code>int</code> - The expression would evaluate to a <code>0</code>.</p>

  <p><code>a</code> is assigned to the value of 1 and <code>b</code> is assigned to the value of 2; and 1 / 2 is 0. The data type here is an <code>int</code> since we are performing integer division.</p>

</details>

<details>
  <summary>Given the expression, <code>a + b > c + d</code>, what would the appropriate data type be? What is the result?</summary>

  <p>Answer:<br><code>boolean</code> - The expression would evaluate to a <code>false</code>.</p>

  <p><code>a</code> is assigned to the value of 1, <code>b</code> is assigned the value of 2, <code>c</code> is assigned the value of 3, and <code>d</code> is assigned the value of 4; and 1 + 2 > 3 + 4 --> 3 > 7 is false.</p>

</details>
