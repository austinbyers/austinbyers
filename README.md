## 🌈 H3ll0 W0rld 👋

I'm a backend software engineer passionate about Go, AWS, serverless, cybersecurity, algorithms, compilers, infrastructure-as-code, musicals, hiking, [Factorio](https://factorio.com), and [XKCD](https://xkcd.com). I've also worked with Python, Java, C#, machine learning, pianos, and trumpets 🎺

If you want to get ahold of me, [LinkedIn](https://www.linkedin.com/in/austinbyers/) works well.


### Parsers
I seem to be enthralled by tedious, recursive, low-level work that might bore others to death - like processing an abstract syntax tree from a compiler.

- If you want to use Python to traverse a JavaScript AST, see my [esprima-ast-visitor](https://github.com/austinbyers/esprima-ast-visitor)
- If you want to translate [LOLCODE](https://en.wikipedia.org/wiki/LOLCODE) into Python and then run it, see [LOLcat](https://github.com/austinbyers/LOLcat)

I highly recommend LOLCODE for your next project. For example, need a [Fibonacci generator](https://github.com/austinbyers/LOLcat/blob/master/fib.lol)?

```
HAI
BTW This program prints every fibonacci number in a specified range
BTW Austin Byers, 2013

	U SEEZ "I will find your fib numbers!\nWhere do U want to start?"
	GIMMEH start_num

	U SEEZ "Where do U want to end?"
	GIMMEH end_num

	OBTW fibonacci is our main variable
		 second_fib is the fib number right before fibonacci 
	TLDR
	I HAS A fibonacci ITZ 1 
	I HAS A second_fib ITZ 1

	I HAS A printflag ITZ FAIL   BTW This means False
	I HAS A finishflag ITZ FAIL

	HOW DUZ I get_next_fib ?
		I HAS A tempvar ITZ fibonacci
		LOL fibonacci IZ NOW fibonacci PLUS second_fib
		LOL second_fib IZ NOW tempvar
	IF U SAY SO
...
```

Still more readable than Haskell.
