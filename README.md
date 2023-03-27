# memo - A daily reminder

memo is a POSIX shell script that stores a small message that will only be 
readable during the day it was stored. It's perfect for sending yourself a 
small daily reminder or motivational phrase you may later show on anything that 
is able to read from standard output.

## Usage

memo accepts this syntax:

```
$ memo [-n]
```

memo stores its message into ``~/.memofile`` by default, but this path may be
changed by setting up an environment variable named ``$MEMO_FILE``.

To store a new memo, use the ``-n`` flag; memo will read the contents from
standard input, so the usual shell utilities may be used to pipe the message
into memo.

Running memo without flags will show the stored message if and only if the date
is the same as the date of storage of the message. The message will be printed
to standard output.

## License

memo is published under an MIT/X11/Expat-type License. See ``LICENSE`` file for 
copyright and license details.
