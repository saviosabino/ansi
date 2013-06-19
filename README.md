ANSI
====

Various ANSI escape codes, used in moving the cursor in a text console or
rendering coloured text.


Example
-------

Print something in bold yellow on a red background:

    >>> from ansi.colour import fg, bg, reset
    >>> print map(str, [bg.red, fg.yellow, 'Hello world!', reset])
    ...

If you like syntactic sugar, you may also do:

    >>> print bg.red(fg.yellow('Hello world!'))
    ...

Also, 256 RGB colours are supported:

    >>> from ansi.colour import rgb, reset
    >>> print rgb(0xff, 0x80, 0x00) + 'hello world' + reset
    ...

If you prefer to use American English in stead:

    >>> from ansi.color import ...
