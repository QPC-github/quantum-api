---
uid: Microsoft.Quantum.ErrorCorrection.EncodeIntoSteaneCode
title: EncodeIntoSteaneCode operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.ErrorCorrection
qsharp.name: EncodeIntoSteaneCode
qsharp.summary: >-
  An encoding operation that maps an unencoded quantum register to an encoded quantum register
  under the ⟦7, 1, 3⟧ Steane quantum code.
---

# EncodeIntoSteaneCode operation

Namespace: [Microsoft.Quantum.ErrorCorrection](xref:Microsoft.Quantum.ErrorCorrection)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


An encoding operation that maps an unencoded quantum register to an encoded quantum registerunder the ⟦7, 1, 3⟧ Steane quantum code.

```qsharp
operation EncodeIntoSteaneCode (physRegister : Qubit[], auxQubits : Qubit[]) : Microsoft.Quantum.ErrorCorrection.LogicalRegister
```


## Input

### physRegister : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

A qubit register which holds the an unencoded quantum state


### auxQubits : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

A qubit register which is initially zero and which gets added to the quantumsystem so that an encoding operation can be performed



## Output : [LogicalRegister](xref:Microsoft.Quantum.ErrorCorrection.LogicalRegister)

A quantum register holding the state after the Steane encoder has been applied

## See Also

- [Microsoft.Quantum.ErrorCorrection.LogicalRegister](xref:Microsoft.Quantum.ErrorCorrection.LogicalRegister)
- [Microsoft.Quantum.ErrorCorrection.SteaneCodeDecoder](xref:Microsoft.Quantum.ErrorCorrection.SteaneCodeDecoder)