---
uid: Microsoft.Quantum.Chemistry.JordanWigner.OptimizedBEXY
title: OptimizedBEXY operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Chemistry.JordanWigner
qsharp.name: OptimizedBEXY
qsharp.summary: >-
  Applies a sequence of Z operations and either an X or Y operation to
  a register of qubits, where the selection of target qubits and basis
  are conditioned on the state of a control register.
---

# OptimizedBEXY operation

Namespace: [Microsoft.Quantum.Chemistry.JordanWigner](xref:Microsoft.Quantum.Chemistry.JordanWigner)

Package: [Microsoft.Quantum.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Chemistry)


Applies a sequence of Z operations and either an X or Y operation toa register of qubits, where the selection of target qubits and basisare conditioned on the state of a control register.

```qsharp
operation OptimizedBEXY (pauliBasis : Qubit, indexRegister : Microsoft.Quantum.Arithmetic.LittleEndian, targetRegister : Qubit[]) : Unit is Adj + Ctl
```


## Description

This operation can be described by a unitary matrix $U$ that appliesthe Pauli string on $(X^{z+1}\_pY^{z}\_p)Z\_{p-1}...Z_0$ onqubits $0..p$ conditioned on an index $z\in\{0,1\}$ and $p$.That is,$$\begin{align}U\ket{z}\ket{p}\ket{\psi} = \ket{z}\ket{p}(X^{z+1}\_pY^{z}\_p)Z\_{p-1}...Z_0\ket{\psi}\end{align}$$

## Input

### pauliBasis : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

When this qubit is in state $\ket{0}$, an `X` operation is applied. When it is in state $\ket{1}$, `Y` is applied.


### indexRegister : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

The state $\ket{p}$ of this register determines the qubit on which `X` or `Y` is applied.


### targetRegister : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Register of qubits on which the Pauli operators are applied.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## References

- Encoding Electronic Spectra in Quantum Circuits with Linear T Complexity  Ryan Babbush, Craig Gidney, Dominic W. Berry, Nathan Wiebe, Jarrod McClean, Alexandru Paler, Austin Fowler, Hartmut Neven  https://arxiv.org/abs/1805.03662