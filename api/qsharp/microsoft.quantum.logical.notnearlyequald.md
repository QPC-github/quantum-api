---
uid: Microsoft.Quantum.Logical.NotNearlyEqualD
title: NotNearlyEqualD function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Logical
qsharp.name: NotNearlyEqualD
qsharp.summary: >-
  Returns true if and only if two inputs are not nearly equal (that is,
  are not within a tolerance of 1e-12).
---

# NotNearlyEqualD function

Namespace: [Microsoft.Quantum.Logical](xref:Microsoft.Quantum.Logical)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns true if and only if two inputs are not nearly equal (that is,are not within a tolerance of 1e-12).

```qsharp
function NotNearlyEqualD (a : Double, b : Double) : Bool
```


## Input

### a : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

The first value to be compared.


### b : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

The second value to be compared.



## Output : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

`true` if and only if `a` is not nearly equal to `b`.

## Remarks

The following are equivalent:```qsharplet cond = Microsoft.Quantum.Math.AbsD(a - b) >= 1e-12;let cond = NotNearlyEqualD(a, b);```