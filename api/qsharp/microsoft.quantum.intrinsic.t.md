---
uid: Microsoft.Quantum.Intrinsic.T
title: T operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: T
qsharp.summary: Applies the π/8 gate to a single qubit.
---

# T operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.Type1.Core](https://nuget.org/packages/Microsoft.Quantum.Type1.Core)


Applies the π/8 gate to a single qubit.

```qsharp
operation T (qubit : Qubit) : Unit is Adj + Ctl
```


## Description

\begin{align}T \mathrel{:=}\begin{bmatrix}1 & 0 \\\\0 & e^{i \pi / 4}\end{bmatrix}.\end{align}

## Input

### qubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit to which the gate should be applied.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

