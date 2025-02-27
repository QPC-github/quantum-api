---
uid: Microsoft.Quantum.Measurement.MeasureWithScratch
title: MeasureWithScratch operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Measurement
qsharp.name: MeasureWithScratch
qsharp.summary: >-
  Measures the given Pauli operator using an explicit scratch
  qubit to perform the measurement.
---

# MeasureWithScratch operation

Namespace: [Microsoft.Quantum.Measurement](xref:Microsoft.Quantum.Measurement)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Measures the given Pauli operator using an explicit scratchqubit to perform the measurement.

```qsharp
operation MeasureWithScratch (pauli : Pauli[], target : Qubit[]) : Result
```


## Input

### pauli : [Pauli](xref:microsoft.quantum.qsharp.valueliterals#pauli-literals)[]

A multi-qubit Pauli operator specified as an array ofsingle-qubit Pauli operators.


### target : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Qubit register to be measured.



## Output : [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal)

The result of measuring the given Pauli operator onthe `target` register.