---
uid: Microsoft.Quantum.Arithmetic.ReversedOpLEC
title: ReversedOpLEC function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: ReversedOpLEC
qsharp.summary: >-
  Given an operation that takes a little-endian input, returns a new
  operation that takes a big-endian input.
---

# ReversedOpLEC function

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given an operation that takes a little-endian input, returns a newoperation that takes a big-endian input.

```qsharp
function ReversedOpLEC (op : (Microsoft.Quantum.Arithmetic.LittleEndian => Unit is Ctl)) : (Microsoft.Quantum.Arithmetic.BigEndian => Unit is Ctl)
```


## Input

### op : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Ctl

The operation whose input is to be reversed.



## Output : [BigEndian](xref:Microsoft.Quantum.Arithmetic.BigEndian) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Ctl

A new operation that accepts its input as a big-endian register.

## See Also

- [Microsoft.Quantum.Arithmetic.ApplyReversedOpLEC](xref:Microsoft.Quantum.Arithmetic.ApplyReversedOpLEC)
- [Microsoft.Quantum.Arithmetic.ReversedOpLE](xref:Microsoft.Quantum.Arithmetic.ReversedOpLE)
- [Microsoft.Quantum.Arithmetic.ReversedOpLEA](xref:Microsoft.Quantum.Arithmetic.ReversedOpLEA)
- [Microsoft.Quantum.Arithmetic.ReversedOpLECA](xref:Microsoft.Quantum.Arithmetic.ReversedOpLECA)