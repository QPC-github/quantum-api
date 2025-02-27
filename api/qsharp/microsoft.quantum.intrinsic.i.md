---
uid: Microsoft.Quantum.Intrinsic.I
title: I operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: I
qsharp.summary: Performs the identity operation (no-op) on a single qubit.
---

# I operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.Type1.Core](https://nuget.org/packages/Microsoft.Quantum.Type1.Core)


Performs the identity operation (no-op) on a single qubit.

```qsharp
operation I (target : Qubit) : Unit is Adj + Ctl
```


## Input

### target : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)





## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

This is a no-op. It is provided for completeness and becausesometimes it is useful to call the identity in an algorithm or to pass it as a parameter.