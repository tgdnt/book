# book

This is an add-on for [todo.sh](https://github.com/todotxt/todo.txt-cli/)
that grabs a todo and creates a calendar event out of it via
[Khal](https://lostpackets.de/khal/).

Usage:

```
todo.sh book ITEM# DATE TIME DURATION
```

Example:

```
todo.sh book 7 2018-06-24 21:42 2h
# Creates an event titled the same as todo number 7,
# on June 24th 2018 from 9:42 PM to 11:42 PM.
```

Notes:

This script takes a date and time in `%Y-%m-%d %H:%M` and automatically
converts it to `%m.%d`, which is what I use for Khal.

This script automatically runs `vdirsyncer sync` to sync your calendar.
