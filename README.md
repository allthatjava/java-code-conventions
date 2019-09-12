# Java Code Conventions 

If not stated here, please follow the [Java Standard Code Convention](https://www.oracle.com/technetwork/java/codeconventions-150003.pdf).

### Code Length

* No more than __80__ characters per line and __2000__ line per page

### JavaDoc

* all __class__ and __public__ method must have __javadoc__. Other methods are optional

### Indentation

* Four spaces should be used as a unit of indentation. Set it on your IDE

### Cleaner Code
* Use 'import static' to make your code cleaner for static vars and methods
* Use `String.format(..)` instead of concatenate with `+` when template can be used (e.g. `String.format("%s is %d years old", "Brian", 29)` )
* Use StringBuilder instead StringBuffer to create/modify String
* Format the code before commit (Eclipse:`Ctrl+Shift+F`, Intellij:`Ctrl+Shift+Alt+L`)

### Conditional statement
* Parenthesis: must be used even if a single line conditional statement
* equals : Constant variable first to avoid NullPointerException (e.g. `if("abc".equals(variable)){...}`)
  * order matters : put lesser possible condition first
* Avoid ternary conditional statement ( with `? :` ).

### Loop Statement

* Avoid: __do-while__ statement.
* Avoid: try to avoid __switch__ statement. If possible, use patterns or functions

### Exception Handling
* Keep throwing the exception to the controller, so error handling can be centralized

### Getter / Setter
* Use the tool provided automation (e.g. In eclipse source > generate getters and setters)
* or Use Lombok : Annotation based

### Unit Test
* Do negative test along with positive test (Include throwing exception)

### Tools
* Must have SonarLint plugin in your IDE (points out what's good or not)

