---
uid: Microsoft.Quantum.Canon.CurriedOp
title: CurriedOp function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: CurriedOp
qsharp.summary: Returns a curried version of an operation on two inputs.
---

# CurriedOp function

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns a curried version of an operation on two inputs.

```qsharp
function CurriedOp<'T, 'U> (op : (('T, 'U) => Unit)) : ('T -> ('U => Unit))
```


## Description

Given an operation with two inputs, this function applies Curry's isomorphism$f(x, y) \equiv f(x)(y)$ to return an operation of one input whichreturns an operation of one input.

## Input

### op : ('T,'U) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) 

An operation whose input is a pair.



## Output : 'T -> 'U => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) 

An operation which accepts the first element of a pair and returnsan operation which accepts as its input the second element of theoriginal operation's input.

## Type Parameters

### 'T

The type of the first component of a function defined on pairs.
### 'U

The type of the second component of a function defined on pairs.

## Remarks

The following are equivalent:```qsharpop(x, y);let curried = CurriedOp(op);let partial = curried(x);partial(y);```

## See Also

- [Microsoft.Quantum.Canon.CurriedOpC](xref:Microsoft.Quantum.Canon.CurriedOpC)
- [Microsoft.Quantum.Canon.CurriedOpA](xref:Microsoft.Quantum.Canon.CurriedOpA)
- [Microsoft.Quantum.Canon.CurriedOpCA](xref:Microsoft.Quantum.Canon.CurriedOpCA)