# REGEX Challenge

### Goal

This lite exercise will help you gain practice in using regular expressions. While all 

problems require you to provide the proper regex, some will require you to also provide 

additional information or research the internet.

### Directions

It's recommended that the student uses https://regex101.com/ when attempting to solve the 

problem set. Put your fully explained solution in this file. 

### Exercises

Provide three regexes that matches `yes yes yes` but not `no no no`

```c#
answer:  \w\w\w\s\w\w\w\s\w\w\w
    OR:  \w{3}\s\w{3}\s\w{3}

```

Provide a regex that matches valid phone numbers with the forms `678-123-1122` and `(678) 

123-1122` while still allowing symbols to be optional. HINT: Research the rules around valid 

phone numbers.

```c#
answer:  .?(\d\d\d).*(\d\d\d).(\d\d\d\d)
    OR:  .?(?:\d{3}.*(?:\d{3}).(?:\d{4})  

```

Provide a regex that matches URLs like `https://regex101.com`, `http://facebook.com` and 

`https://www.godaddy.com` but not `https://msdn.microsoft.com`. (Trailing `/` should be 

allowed and optional)

```c#
answer: http\w?:\/\/(\w{3}\.|)(\w*|.?)(\.com)

//This will capture "http//" or "https//"
//This will capture "www." or blank, and nothing else(like "msdn.") 
//This will capture any length of word following line 33
//This will capture ending ".com" only
```

Provide a regex that matches dates with the format: `Wed Aug 11, 2013`.

```c#
answer: (?<DotW>\w{3})\w*\s(?<Month>\w{3})\w*\s(?<Day>\d*),\s(?<Year>\d{4})

//Even if the user spells out day of the week and month, will capture only the first three 

characters 

```

Provide a regex that matches dates with the format: `MM/DD/YYYY`. Use named captures to 

extract Day, Month and Year.

```c#
answer: (?<M>\d\d)\/(?<D>\d\d)\/(?<Y>\d{4})

```

Provide a regex that matches `function returnOne() {return 1;}` and captures the value 

returned.

```c#
answer: function\s+\w+\(\)(?:|\s+|\s+\n)\{(?:\s+\w+\s+|\w+\s+)(?<returnValue>\w+)\;(?:\}|\s

+\}|\n\})

//will capture the return value no matter the spacing/tabbing/cartridge return

```

Provide a regex that matches `List<int> my_List = new List<int>();` and captures the 

variable name.

```c#
answer: \w+\<\w+\>\s+(?<varName>\w+)\s*=\s*new\s*\w+\<\w+\>\(\);

// \s* will accomodate some variation in spacing

```

Provide two regeesx that matches `Billy Jean` but not `billy jean`.

```c#
answer:

```

Provide two regexes that matches `NSS Evening Cohort 3` and captures "Cohort 3".

```c#
answer:

```

Provide a regex that matches emails of the forms `first.last@example.com` and 

`something99@history.com`. Allow for numbers in the domain name as well as the email prefix. 

Capture the domain name.

```c#
answer:

```

Provide a regex (as if for a password checker), that enforces a password to have at least 

one symbol and one number.

```c#
answer:

```

Provide a regex that matches emails from the domains `.com`, `.org`, `.net`, `.io` and `.ly` 

but not `.biz` and `.com.uk`. This regex should capture the end result. (use #10 as a 

starting point).

```c#
answer:

```

Provide a regex that matches the entire [2nd paragraph of the Wikipedia page about John 

Lennon](https://en.wikipedia.org/wiki/John_Lennon).

```c#
answer:

```

Provide a regex that matches the numbered exercises from this challenge.

```c#
answer:

```

Provide two regexes that matches the following C# code and captures the property names. 

(HINT: How could you match a newline?)

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
