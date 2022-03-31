# is-leap-year

Different js functions to find leap years

## Stackoverflow

I was confused by different answers in the following Stackoverflow questions & answers:

 - [javascript to find leap year](https://stackoverflow.com/questions/8175521/javascript-to-find-leap-year)
 - [How to find leap year programmatically in C](https://stackoverflow.com/questions/3220163/how-to-find-leap-year-programmatically-in-c)
 - [Check if year is leap year in javascript [duplicate]](https://stackoverflow.com/questions/16353211/check-if-year-is-leap-year-in-javascript)


## 3 different approaches

ℹ️ They have different result only on year `0` (zero)

1. with `Date()`:

       return (new Date(year, 1, 29).getMonth() == 1);

2. with math calculations:

       return ((year & 3) == 0 && ((year % 25) != 0 || (year & 15) == 0));

3. with math calculations II:

       return ((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0);
