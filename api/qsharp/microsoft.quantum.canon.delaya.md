---
uid: Microsoft.Quantum.Canon.DelayA
title: DelayA operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: DelayA
qsharp.summary: Applies a given operation with a delay.
---

# DelayA operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies a given operation with a delay.

```qsharp
operation DelayA<'T> (op : ('T => Unit is Adj), arg : 'T, aux : Unit) : Unit is Adj
```


## Description

Given an operation and an input to that operation, appliesthe operation once an additional input is provided.In particular, the expression `Delay(op, arg, _)` is an operation thatapplies `op` to `arg` when called.Expression `Delay(op,arg,_)` allows to delay the application of `op`.

## Input

### op : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

An operation to be applied.


### arg : 'T

The input to which the operation is applied.


### aux : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

Argument used to delay the application of operation by usingpartial application.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The input type of the operation to be delayed.

## See Also

- [Microsoft.Quantum.Canon.Delay](xref:Microsoft.Quantum.Canon.Delay)
- [Microsoft.Quantum.Canon.Delayed](xref:Microsoft.Quantum.Canon.Delayed)