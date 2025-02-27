---
uid: Microsoft.Quantum.Diagnostics.DumpOperation
title: DumpOperation operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Diagnostics
qsharp.name: DumpOperation
qsharp.summary: >-
  Given an operation, displays diagnostics about
  the operation that are made available by the current
  execution target.
---

# DumpOperation operation

Namespace: [Microsoft.Quantum.Diagnostics](xref:Microsoft.Quantum.Diagnostics)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given an operation, displays diagnostics aboutthe operation that are made available by the currentexecution target.

```qsharp
operation DumpOperation (nQubits : Int, op : (Qubit[] => Unit is Adj)) : Unit is Adj + Ctl
```


## Input

### nQubits : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of qubits on which the given operation acts.


### op : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[] => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

The operation that is to be diagnosed.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Example

When run on the quantum simulator target, the following snippet willoutput the matrix$$\begin{aligned}\left(\begin{matrix}1 & 0 & 0 & 0 \\\\0 & 0 & 0 & 1 \\\\0 & 0 & 1 & 0 \\\\0 & 1 & 0 & 0\end{matrix}\right)\end{aligned}.$$```qsharpoperation DumpCnot() : Unit {    DumpOperation(2, ApplyToFirstTwoQubitsCA(CNOT, _));}```

## Remarks

Calling this operation has no observable effect from withinQ#. The exact diagnostics that are displayed, if any, aredependent on the current execution target and editor environment.For example, when used on the full-state quantum simulator,a unitary matrix used to represent `op` is displayed.Note that, when run on simulators that admit a global phase ambiguity(e.g.: the full-state simulator), returned representations may varyup to a global phase.Similarly, the ordering of rows and columns matrix representationsmay vary with the conventions used by each simulator supporting thisoperation.