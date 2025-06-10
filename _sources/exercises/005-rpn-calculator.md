# 005 - Reverse Polish Notation (RPN) Calculator

In this exercise you will implement a simple RPN calculator similar to
the unix 'dc' command.

See the [Wikipedia page](https://en.wikipedia.org/wiki/Reverse_Polish_notation)
for full information on the syntax.

  * Each time a number is entered, it is pushed onto a [**stack**](https://en.wikipedia.org/wiki/Stack_(abstract_data_type))
  * The **stack** is an ordered set of numbers and it is managed as "Last In First Out" queue.
  * If an operater is entered, such as {+,-,*,/} the last two numbers entered on the stack are removed and used as the operands for the operator. The result of that calculation is pushed onto the top of the stack.

  For this exercise you should implement an RPN calculator in python which
handles (at least) integer inputs and following single character commands:

  * `+` - Remove the top two values from the stack, add them and push that onto the stack
  * `*` - Remove the top two values from the stack, multiply them and push that onto the stack
  * `-` - Remove the top two values from the stack, substract the latest one from the penultimate one and push the result onto the stack
  * `\` - Remove the top two values from the stack, divide the penultimate one by the latest one and push the result onto the stack
  * `f` - Print the entire stack
  * `p` - Print the top element in the stack but leaves it on the stack (peek)
  * `P` - Print the top element in the stack and removes it from the stack (pop)
  * `c` - Clear the stack
  * `q` - Exit the program

![HP 32S](../assets/Hp-32s.jpg)


