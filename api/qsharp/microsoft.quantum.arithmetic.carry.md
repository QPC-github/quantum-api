---
uid: Microsoft.Quantum.Arithmetic.Carry
title: Carry operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: Carry
qsharp.summary: >-
  Implements a reversible carry gate. Given a carry-in bit encoded in
  qubit `carryIn` and two summand bits encoded in `summand1` and `summand2`,
  computes the bitwise xor of `carryIn`, `summand1` and `summand2` in the
  qubit `summand2` and the carry-out is xored to the qubit `carryOut`.
---

# Carry operation

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Implements a reversible carry gate. Given a carry-in bit encoded inqubit `carryIn` and two summand bits encoded in `summand1` and `summand2`,computes the bitwise xor of `carryIn`, `summand1` and `summand2` in thequbit `summand2` and the carry-out is xored to the qubit `carryOut`.

```qsharp
operation Carry (carryIn : Qubit, summand1 : Qubit, summand2 : Qubit, carryOut : Qubit) : Unit is Adj + Ctl
```


## Input

### carryIn : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Carry-in qubit.


### summand1 : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

First summand qubit.


### summand2 : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Second summand qubit, is replaced with the lower bit of the sum of`summand1` and `summand2`.


### carryOut : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Carry-out qubit, will be xored with the higher bit of the sum.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

