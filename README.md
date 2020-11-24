## 🌈 H3ll0 W0rld 👋

I'm a backend software engineer passionate about Go, serverless, cybersecurity, algorithms, compilers, musicals, hiking, [Factorio](https://factorio.com), [XKCD](https://xkcd.com), [the gay agenda](https://www.sfgmc.org/), lists, and Oxford commas. I've also worked with Python, Java, C#, machine learning, pianos, and trumpets 🎺

If you want to get ahold of me, [LinkedIn](https://www.linkedin.com/in/austinbyers/) works well.

### Open-Source Security

My entire professional career thus far has been spent building serverless security tools in AWS infrastructure:

- 🐈 I'm the founding backend engineer for [Panther](https://github.com/panther-labs/panther), an open-source serverless security platform for log processing, real-time alerting and remediation, and [other cool stuff](https://runpanther.io). I specialize in the developer tooling, API layer, and premium features.
- 🐞 I'm the original author of Airbnb's [BinaryAlert](https://github.com/airbnb/binaryalert), which provides serverless scalable malware detection with [YARA rules](https://virustotal.github.io/yara/).
- ⚠️ I've also made some contributions to Airbnb's [StreamAlert](https://github.com/airbnb/streamalert), which provides a Python interface for real-time log matching - a kind of spiritual predecessor to Panther.


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


### Other Fun Stuff

A Python [quine](https://en.wikipedia.org/wiki/Quine_(computing)):

```python
q1='"'
q2="'"
src="print('q1=' + q2 + q1 + q2); print('q2=' + q1 + q2 + q1); print('src=' + q1 + src + q1); print(src)"
print('q1=' + q2 + q1 + q2); print('q2=' + q1 + q2 + q1); print('src=' + q1 + src + q1); print(src)
```

And another one in Go:

```go
package main

import "fmt"

var src = `func main() {
	fmt.Printf("package main\n\n")
	fmt.Printf("import \"fmt\"\n\n")
	fmt.Printf("var src = %s%s%s\n\n", string(96), src, string(96))
	fmt.Println(src)
}
`

func main() {
	fmt.Printf("package main\n\n")
	fmt.Printf("import \"fmt\"\n\n")
	fmt.Printf("var src = %s%s%s\n\n", string(96), src, string(96))
	fmt.Println(src)
}

```

Finally, a message to my former self when I see my old code:

```go
package main

import (
	"fmt"
	"time"
)

type x struct{}

func (x) self() {
	fmt.Println("#GoFuncYourSelf")
}

func main() {
	var your x
  
	go func() { your.self() }()  
  
	time.Sleep(1)
}
```
