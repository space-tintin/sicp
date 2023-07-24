# Chapter 1
--- 

**Based SWE**
- Organize programs to be deterministic  
- Visualize the behavior of a system  
- Debug programs  
- Write programs to be modular  
- Structure programs to not be catastrophic (Fail gracefully)  

## 1.1 Elements of Programming

**Mechanisms of programming**
- Primitives (ya know, numbers and stuff)  
- Combinations (build stuff out of primitives)  
- Abstractions (Names and manipulations of combinations)  

**Elements**  
- Procedures (Descriptions of rules for manipulating data)  
- Data (Stuff to manipulate)  

### 1.1.1 Expressions

**Notations**
Prefix Notation: `(+ 1 2)`, `(operator, operand, operand)`
Infix Notation: `1 + 2`, `(operand, operator, operand)` 
Postfix Notation: `1 2 +`, `(operand, operand, operator)`

Scheme, Python, and Rust all use prefix notation.


### 1.1.2 Naming and the Environment

**Variables**
Variables are abstractions assigning a name to a primitive or combination. In the case of scheme this is done with the `define` keyword. In python this is done with the `=` operator. in rust this is done with the `let` keyword (and `=` operator).

Scheme: `(define x 1)`
Python: `x = 1`
Rust: `let x = 1;`

**Environment**
Using variable abstraction consumes memory. The memory of a program is called the global environment

### 1.1.3 Evaluating Combinations

Evaluation procedure:  
1. Evaluate the subexpressions of the combination  
2. Apply the operator to the operand  

There are problems with thinking procedurally:  

