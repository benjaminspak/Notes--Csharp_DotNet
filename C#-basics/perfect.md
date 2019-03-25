### Problem Solving Steps - Prefect

- if / else if / else -- Same as JS.
- "try" Code and "catch" Exceptions -- Same as JS.

#### Doubles

- `_double_` (float) type: a numeric data type used to store decimal values.

#### Working With Numbers

- Casting: changing a float type to an int
- Truncation (While casting): Rather than round up the numerals after the decimal are removed.

```C#
(int)2.9  // Original cast
2  // Truncated value
 ```

- The result of two ints is always an int. Even if there is a remainder.

```C#
7 / 3  // Actual result 2.3(Repeated 3)
2  // Truncated result
```

- Double’s can’t be stored in integers without a cast.

```C#
int x = 2.9  // Will result in a compilation error
```

- The following will not be stored because the double (float) is not cast.

```C#
int x = 9 / 6.0;
int x = (int)9 / 6.0;
```

- The following will be stored.

```C#
int x = (int)(9 / 6.0)
```

#### Avoiding type names

- You can use `var` to declare a variable as long as the variable type is explicit.

```C#
// string input = "22";
var input = "22";
// int converted = int.Parse(input);
var converted = int.Parse(input);
// bool wheelsAreRound = true;
var wheelsAreRound = true;
// string downcased = "DoNuTs".ToLower();
var downcased = "DoNuTs".ToLower();
// bool success = (downcased == "donuts");
var success = (downcased == "donuts");
// double total = 0;
var total = 0.0;
```