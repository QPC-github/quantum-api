---
uid: Microsoft.Quantum.Intrinsic.M
title: M operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: M
qsharp.summary: >-
  Performs a measurement of a single qubit in the
  Pauli $Z$ basis.
---

# M operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.Type1.Core](https://nuget.org/packages/Microsoft.Quantum.Type1.Core)


Performs a measurement of a single qubit in thePauli $Z$ basis.

```qsharp
operation M (qubit : Qubit) : Result
```


## Description

The output result is given bythe distribution\begin{align}\Pr(\texttt{Zero} | \ket{\psi}) =\braket{\psi | 0} \braket{0 | \psi}.\end{align}

## Input

### qubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit to be measured.



## Output : [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal)

`Zero` if the $+1$ eigenvalue is observed, and `One` ifthe $-1$ eigenvalue is observed.

## Remarks

Equivalent to:```qsharpMeasure([PauliZ], [qubit]);```