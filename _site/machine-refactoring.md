# Machine Powered Refactoring

Amal Hussein, Bocoup

- Web Platform Podcast
- Love unit testing

### Themes

- "Rapid innovation comes with price"
- "A plea for ~~better~~ **prioritization** of application maintenance"


## Application Maintenance Dilemmas

- Code cruft
- Aging and shifting dependencies
- Growing and unruly code bases
- Insufficient unit and integration test coverage

![node module weight](https://i.redd.it/tfugj4n3l6ez.png)



## Abstract Syntax Trees (ASTs)

- [astexplorer.net](astexplorer.net)
- "n computer science, an abstract syntax tree (AST), or just syntax tree, is a tree representation of the abstract syntactic structure of source code written in a programming language. Each node of the tree denotes a construct occurring in the source code." - [wikipedia](https://en.wikipedia.org/wiki/Abstract_syntax_tree)

![ast](https://slideplayer.com/slide/5087012/16/images/2/Abstract+Syntax+Tree+%2B+%2A+if-statement+if-statement+can+become+IF+cond.jpg)

### Compilers

![compiler](http://creativejs.com/wp-content/uploads/2013/05/Compiler-architecture.png)

### AST Compilers power our tools

- Babel
    - 100% volunteer
    - ![babel](https://dab1nmslvvntp.cloudfront.net/wp-content/uploads/2016/04/1459949808babel.png)
    - [Understanding Babel](https://www.sitepoint.com/understanding-asts-building-babel-plugin/)
    - [preval](https://github.com/kentcdodds/babel-plugin-preval)
        ```
        const x = preval`module.exports = 1`

        //      ↓ ↓ ↓ ↓ ↓ ↓

        const x = 1
```
- Lint
    - JSHint
        - https://addyosmani.com/blog/fixmyjs/
        - ![image](https://addyosmani.com/assets/jshint.png)
- Istanbul


## Automate Pyramid on Defect (Patterns of Defense)

1. Write custom lint rule
1. Write a unit test
1. Write an integration test


## Use [AST Explorer](https://astexplorer.net/)

- [jsCodeShift](https://github.com/facebook/jscodeshift)


## Questions

- Ensure that your translations don't cause bugs
    - Use unit tests
    - Be tight with you `codemon`s
