---
uid: Microsoft.Quantum.Intrinsic.Rx
title: Rx operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: Rx
qsharp.summary: ''
---

# Rx operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.Type1.Core](https://nuget.org/packages/Microsoft.Quantum.Type1.Core)




```qsharp
operation Rx (theta : Double, qubit : Qubit) : Unit is Adj + Ctl
```


## Description

\begin{align}R_x(\theta) \mathrel{:=}e^{-i \theta \sigma_x / 2} =\begin{bmatrix}\cos \frac{\theta}{2} & -i\sin \frac{\theta}{2}  \\\\-i\sin \frac{\theta}{2} & \cos \frac{\theta}{2}\end{bmatrix}.\end{align}

## Input

### theta : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Angle about which the qubit is to be rotated.


### qubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit to which the gate should be applied.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

Equivalent to:```qsharpR(PauliX, theta, qubit);```