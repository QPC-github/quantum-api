---
uid: Microsoft.Quantum.Measurement.SetToBasisState
title: SetToBasisState operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Measurement
qsharp.name: SetToBasisState
qsharp.summary: >-
  Sets a qubit to a given computational basis state by measuring the
  qubit and applying a bit flip if needed.
---

# SetToBasisState operation

Namespace: [Microsoft.Quantum.Measurement](xref:Microsoft.Quantum.Measurement)

Package: [Microsoft.Quantum.Type1.Core](https://nuget.org/packages/Microsoft.Quantum.Type1.Core)


Sets a qubit to a given computational basis state by measuring thequbit and applying a bit flip if needed.

```qsharp
operation SetToBasisState (desired : Result, target : Qubit) : Unit
```


## Input

### desired : [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal)

The basis state that the qubit should be set to.


### target : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

The qubit whose state is to be set.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

As an invariant of this operation, calling `M(q)` immediatelyafter `SetToBasisState(result, q)` will return `result`.