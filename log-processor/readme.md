## Process the log

### What you need to do

* If you haven’t used git before, take a [git class in codeschool](https://www.codeschool.com/courses/try-git).
* Once complete, create a private repo called “yipl-se-log-processor” in [bitbucket](https://bitbucket.org)
* Solve the problem detailed below
* Push your code to the repo (make sure that you have multiple commits with proper messages) 
* Invite applications-bitbucket@yipl.com.np to that particular private repo
* Submit your application

#### Problem

You need to write code that reads the given [log](example.log) [files](example1.log) (passed as an argument from cli), processes its content and provides a summary of the logs, as shown in the 'output' section below. The code should accept any number of log files from the command line. The code should be written in any one of the following programming languages: node, python, php, golang. 

The filename should be: process.php, process.py, process.js or process.go depending upon the language you choose.

Your code should run from the cli as shown below. If you don’t know how to use cli in one of the given languages, now is the time to learn it. 

In php, 
`php process.php -f example.log example1.log`

In python, 
`python process.py  -f example.log example1.log`

In node,
`node process.js -f example.log example1.log`

In go,
`go run process.go -f example.log example1.log`

Running the above command should give the following output:
```
2016-12-12 warning:2 error: 1
2016-12-13 warning:0 error: 1
2016-12-14 warning:2 error: 1
2016-12-15 warning:1 error: 0
2016-12-16 warning:0 error: 1
```

### Further instruction

* Create a separate class file. Your class filename should be "logprocessor.php", "logprocessor.py" and so on for other languages. 
* Write readme file with the instructions necessary to run the code


### Bonus points

* If you can write and include unit tests for your code. 
