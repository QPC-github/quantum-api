---
uid: Microsoft.Quantum.Arithmetic.ApplyPhaseLEOperationOnLEA
title: ApplyPhaseLEOperationOnLEA operation
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: ApplyPhaseLEOperationOnLEA
qsharp.summary: >-
  Applies an operation that takes a
  <xref:Microsoft.Quantum.Arithmetic.LittleEndian> register as input
  on a target register of type <xref:Microsoft.Quantum.Arithmetic.PhaseLittleEndian>.
---

# ApplyPhaseLEOperationOnLEA operation

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies an operation that takes a<xref:Microsoft.Quantum.Arithmetic.LittleEndian> register as inputon a target register of type <xref:Microsoft.Quantum.Arithmetic.PhaseLittleEndian>.

```qsharp
operation ApplyPhaseLEOperationOnLEA (op : (Microsoft.Quantum.Arithmetic.PhaseLittleEndian => Unit is Adj), target : Microsoft.Quantum.Arithmetic.LittleEndian) : Unit is Adj
```


## Input

### op : [PhaseLittleEndian](xref:Microsoft.Quantum.Arithmetic.PhaseLittleEndian) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

The operation to be applied.


### target : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

The register to which the operation is applied.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

The register is transformed to `PhaseLittleEndian` by the use of<xref:Microsoft.Quantum.Canon.QFTLE> and is then returned toits original representation after application of `op`.

## See Also

- [Microsoft.Quantum.Arithmetic.ApplyPhaseLEOperationOnLE](xref:Microsoft.Quantum.Arithmetic.ApplyPhaseLEOperationOnLE)
- [Microsoft.Quantum.Arithmetic.ApplyPhaseLEOperationOnLEC](xref:Microsoft.Quantum.Arithmetic.ApplyPhaseLEOperationOnLEC)
- [Microsoft.Quantum.Arithmetic.ApplyPhaseLEOperationOnLECA](xref:Microsoft.Quantum.Arithmetic.ApplyPhaseLEOperationOnLECA)