---
uid: Microsoft.Quantum.Canon.ApplyToEachC
title: ApplyToEachC operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyToEachC
qsharp.summary: >-
  Applies a single-qubit operation to each element in a register.
  The modifier `C` indicates that the single-qubit operation is controllable.
---

# ApplyToEachC operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies a single-qubit operation to each element in a register.The modifier `C` indicates that the single-qubit operation is controllable.

```qsharp
operation ApplyToEachC<'T> (singleElementOperation : ('T => Unit is Ctl), register : 'T[]) : Unit is Ctl
```


## Input

### singleElementOperation : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Ctl

Operation to apply to each qubit.


### register : 'T[]

Array of qubits on which to apply the given operation.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The target on which the operation acts.

## Example

Prepare a three-qubit $\ket{+}$ state:```qsharpusing (register = Qubit[3]) {    ApplyToEachC(H, register);}```

## See Also

- [Microsoft.Quantum.Canon.ApplyToEach](xref:Microsoft.Quantum.Canon.ApplyToEach)