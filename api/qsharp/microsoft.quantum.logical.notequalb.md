---
uid: Microsoft.Quantum.Logical.NotEqualB
title: NotEqualB function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Logical
qsharp.name: NotEqualB
qsharp.summary: Returns true if and only if two inputs are not equal.
---

# NotEqualB function

Namespace: [Microsoft.Quantum.Logical](xref:Microsoft.Quantum.Logical)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns true if and only if two inputs are not equal.

```qsharp
function NotEqualB (a : Bool, b : Bool) : Bool
```


## Input

### a : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

The first value to be compared.


### b : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

The second value to be compared.



## Output : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

`true` if and only if `a` is not equal to `b`.

## Remarks

The following are equivalent:```qsharplet cond = a != b;let cond = NotEqualB(a, b);```