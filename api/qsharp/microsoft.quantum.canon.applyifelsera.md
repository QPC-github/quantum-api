---
uid: Microsoft.Quantum.Canon.ApplyIfElseRA
title: ApplyIfElseRA operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyIfElseRA
qsharp.summary: >-
  Applies one of two adjointable operations, depending on the value of a
  classical result.
---

# ApplyIfElseRA operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies one of two adjointable operations, depending on the value of aclassical result.

```qsharp
operation ApplyIfElseRA<'T, 'U> (result : Result, (zeroOp : ('T => Unit is Adj), zeroInput : 'T), (oneOp : ('U => Unit is Adj), oneInput : 'U)) : Unit is Adj
```


## Description

Given a result `result`, applies the operation `zeroOp` with `zeroInput` asits input when `result` is equal to `Zero`, and applies `oneOp(oneInput)`when `result == One`.

## Input

### result : [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal)

The measurement result used to determine if `zeroOp` or `oneOp` isapplied.


### zeroOp : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

The adjointable operation to be applied when `result == Zero`.


### zeroInput : 'T

The input to be provided to `zeroOp` when `result == Zero`.


### oneOp : 'U => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

The adjointable operation to be applied when `result == One`.


### oneInput : 'U

The input to be provided to `oneOp` when `result == One`.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The input type of the operation `zeroOp` to be conditionally applied.
### 'U

The input type of the operation `oneOp` to be conditionally applied.

## See Also

- [Microsoft.Quantum.Canon.ApplyIfZero](xref:Microsoft.Quantum.Canon.ApplyIfZero)
- [Microsoft.Quantum.Canon.ApplyIfOne](xref:Microsoft.Quantum.Canon.ApplyIfOne)
- [Microsoft.Quantum.Canon.ApplyIfElseRC](xref:Microsoft.Quantum.Canon.ApplyIfElseRC)
- [Microsoft.Quantum.Canon.ApplyIfElseRA](xref:Microsoft.Quantum.Canon.ApplyIfElseRA)
- [Microsoft.Quantum.Canon.ApplyIfElseRCA](xref:Microsoft.Quantum.Canon.ApplyIfElseRCA)