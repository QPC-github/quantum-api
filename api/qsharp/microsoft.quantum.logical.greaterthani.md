---
uid: Microsoft.Quantum.Logical.GreaterThanI
title: GreaterThanI function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Logical
qsharp.name: GreaterThanI
qsharp.summary: Returns true if and only if a number is greater than another number.
---

# GreaterThanI function

Namespace: [Microsoft.Quantum.Logical](xref:Microsoft.Quantum.Logical)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns true if and only if a number is greater than another number.

```qsharp
function GreaterThanI (a : Int, b : Int) : Bool
```


## Input

### a : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The first value to be compared.


### b : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The second value to be compared.



## Output : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

`true` if and only if `a` is strictly greater than `b`.

## Remarks

The following are equivalent:```qsharplet cond = a > b;let cond = GreaterThanI(a, b);```