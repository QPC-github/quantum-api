---
uid: Microsoft.Quantum.Intrinsic.R1
title: R1 operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: R1
qsharp.summary: Applies a rotation about the $\ket{1}$ state by a given angle.
---

# R1 operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.Type1.Core](https://nuget.org/packages/Microsoft.Quantum.Type1.Core)


Applies a rotation about the $\ket{1}$ state by a given angle.

```qsharp
operation R1 (theta : Double, qubit : Qubit) : Unit is Adj + Ctl
```


## Description

\begin{align}R_1(\theta) \mathrel{:=}\operatorname{diag}(1, e^{i\theta}).\end{align}

## Input

### theta : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Angle about which the qubit is to be rotated.


### qubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit to which the gate should be applied.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

Equivalent to:```qsharpR(PauliZ, theta, qubit);R(PauliI, -theta, qubit);```