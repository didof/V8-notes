# V8 Notes

My happy island where I keep track of everything about v8 that passes under my nose.

## Index

1. Overiview
2. Parsing

---

## Overivew

```
JS => parser -> AST => Interpreter Ignition -> bytecode

bytecode -> execution
    |
    V
Compiler TurboFan -> optimized machine code
```

> Bytecode is an abstraction of machine code. Compiling bytecode to machine code is easier if the bytecode was designed with the same computational model as the physical CPU. This is why interpreters are often register or stack machines. Ignition is a register machine with an accumulator register. [Franziska Hinkelmann][1]

V8 bytecodes: [bytecodes.h][2]

<!-- links -->

[1]: https://medium.com/dailyjs/understanding-v8s-bytecode-317d46c94775 'Franziska Hinkelmann'
[2]: https://github.com/v8/v8/blob/master/src/interpreter/bytecodes.h 'bytecodes.h'

<!-- [![Franziska Hinkelmann](https://medium.com/dailyjs/understanding-v8s-bytecode-317d46c94775)][1] -->

---
