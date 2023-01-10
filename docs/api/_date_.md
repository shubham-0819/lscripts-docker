---
tilte: lsd module _docs_
description: lsd module _docs_ description
---


# lsd module _docs_

This is a set of Bash functions for working with dates. The functions are * all prefixed with `lsd-mod.date.get` and have different suffixes indicating what kind of date format they return.

* `lsd-mod.date.get()` returns the date in the format "day-month-year, day of the week", for example "11-Jan-2022, Sunday"

* `lsd-mod.date.get__blog()` returns the date and time in the format "year-month-day hour:minute:second", for example "2022-01-11 12:34:56"

* `lsd-mod.date.get__blog-post`() returns the date in the format "year-month-day", for example "2022-01-11"

* `lsd-mod.date.get__full()` returns the date and time in the format "hour:minute:second, day-month-year, day of the week", for example "12:34:56, 11-Jan-2022, Sunday"

* `lsd-mod.date.get__timestamp()` returns a timestamp of the current date and time in the format "daymonthyear_hourminutesecond", for example "110122_123456"

* `lsd-mod.date.get__timestamp_millisec()` returns a timestamp with milliseconds in the format "daymonthyear_hourminutesecond_millisecond", for example "110122_123456_053"

* `lsd-mod.date.get__timestamp_microsec()` returns a timestamp with microseconds in the format "daymonthyear_hourminutesecond_microseconds", for example "110122_123456_053993"

* `lsd-mod.date.get__timestamp_nanosec()` returns a timestamp with nanoseconds in the format "daymonthyear_hourminutesecond_nanoseconds", for example "110122_123456_053993752"

It's worth noting that the date -d now option is used in some of the functions here to get the current date and time, instead of just using date on its own. This is useful when you want to get the date and time at a specific point in time other than the current time, for example: date -d "2022-01-11 12:34:56" will return the date and time on given.
