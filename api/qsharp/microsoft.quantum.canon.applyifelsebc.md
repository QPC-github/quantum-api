---
uid: Microsoft.Quantum.Canon.ApplyIfElseBC
title: ApplyIfElseBC operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyIfElseBC
qsharp.summary: >-
  Applies one of two controllable operations, depending on the value of a
  classical bit.
---

# ApplyIfElseBC operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies one of two controllable operations, depending on the value of aclassical bit.

```qsharp
operation ApplyIfElseBC<'T, 'U> (bit : Bool, (trueOp : ('T => Unit is Ctl), trueInput : 'T), (falseOp : ('U => Unit is Ctl), falseInput : 'U)) : Unit is Ctl
```


## Description

Given a bit `bit`, applies the operation `trueOp` with `trueInput` asits input when `bit` is `true`, and applies `falseOp(falseInput)`when `bit` is `false`.

## Input

### bit : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

The boolean value used to determine whether `trueOp` or `falseOp` isapplied.


### trueOp : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Ctl

The controllable operation to be applied when `bit` is `true`.


### trueInput : 'T

The input to be provided to `trueOp` when `bit` is `true`.


### falseOp : 'U => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Ctl

The controllable operation to be applied when `bit` is `false`.


### falseInput : 'U

The input to be provided to `falseOp` when `bit` is `false`.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The input type of the operation `trueOp` to be conditionally applied.
### 'U

The input type of the operation `falseOp` to be conditionally applied.

## See Also

- [Microsoft.Quantum.Canon.ApplyIfZero](xref:Microsoft.Quantum.Canon.ApplyIfZero)
- [Microsoft.Quantum.Canon.ApplyIfOne](xref:Microsoft.Quantum.Canon.ApplyIfOne)
- [Microsoft.Quantum.Canon.ApplyIfElseRC](xref:Microsoft.Quantum.Canon.ApplyIfElseRC)
- [Microsoft.Quantum.Canon.ApplyIfElseRA](xref:Microsoft.Quantum.Canon.ApplyIfElseRA)
- [Microsoft.Quantum.Canon.ApplyIfElseRCA](xref:Microsoft.Quantum.Canon.ApplyIfElseRCA)