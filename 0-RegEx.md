# REGEX Challenge

### Goal

This lite exercise will help you gain practice in using regular expressions. While all problems require you to provide the proper regex, some will require you to also provide additional information or research the internet.

### Directions

It's recommended that the student uses https://regex101.com/ when attempting to solve the problem set. Put your fully explained solution in this file. 

### Exercises

Provide three regexes that matches `yes yes yes` but not `no no no`

```c#
answer:

```

Provide a regex that matches valid phone numbers with the forms `678-123-1122` and `(678) 123-1122` while still allowing symbols to be optional. HINT: Research the rules around valid phone numbers.

```c#
answer:

```

Provide a regex that matches URLs like `https://regex101.com`, `http://facebook.com` and `https://www.godaddy.com` but not `https://msdn.microsoft.com`. (Trailing `/` should be allowed and optional)

```c#
answer:

```

Provide a regex that matches dates with the format: `Wed Aug 11, 2013`.

```c#
answer:

```

Provide a regex that matches dates with the format: `MM/DD/YYYY`. Use named captures to extract Day, Month and Year.

```c#
answer:

```

Provide a regex that matches `function returnOne() {return 1;}` and captures the value returned.

```c#
answer:

```

Provide a regex that matches `List<int> my_List = new List<int>();` and captures the variable name.

```c#
answer:

```

Provide two regeesx that matches `Billy Jean` but not `billy jean`.

```c#
answer:

```

Provide two regexes that matches `NSS Evening Cohort 3` and captures "Cohort 3".

```c#
answer:

```

Provide a regex that matches emails of the forms `first.last@example.com` and `something99@history.com`. Allow for numbers in the domain name as well as the email prefix. Capture the domain name.

```c#
answer:

```

Provide a regex (as if for a password checker), that enforces a password to have at least one symbol and one number.

```c#
answer:

```

Provide a regex that matches emails from the domains `.com`, `.org`, `.net`, `.io` and `.ly` but not `.biz` and `.com.uk`. This regex should capture the end result. (use #10 as a starting point).

```c#
answer:

```

Provide a regex that matches the entire [2nd paragraph of the Wikipedia page about John Lennon](https://en.wikipedia.org/wiki/John_Lennon).

```c#
answer:

```

Provide a regex that matches the numbered exercises from this challenge.

```c#
answer:

```

Provide two regexes that matches the following C# code and captures the property names. (HINT: How could you match a newline?)

```c#
public class Part
{
    public string PartName { get; set; }
    public int PartId { get; set; }
}
```

```c#
answer:

```
