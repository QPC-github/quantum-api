---
uid: Microsoft.Quantum.Arithmetic.BigEndian
title: BigEndian user defined type
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: udt
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: BigEndian
qsharp.summary: >-
  Register that encodes an unsigned integer in big-endian order. The
  qubit with index `0` encodes the highest bit of an unsigned integer.
---

# BigEndian user defined type

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Register that encodes an unsigned integer in big-endian order. Thequbit with index `0` encodes the highest bit of an unsigned integer.

```qsharp

newtype BigEndian = (Qubit[]);
```



## Remarks

We abbreviate `BigEndian` as `BE` in the documentation.