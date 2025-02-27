---
uid: Microsoft.Quantum.Math.MinI
title: MinI function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Math
qsharp.name: MinI
qsharp.summary: Returns the smaller of two specified numbers.
---

# MinI function

Namespace: [Microsoft.Quantum.Math](xref:Microsoft.Quantum.Math)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Returns the smaller of two specified numbers.

```qsharp
function MinI (a : Int, b : Int) : Int
```


## Input

### a : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The first number to be compared.


### b : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The second number to be compared.



## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The smaller of `a` and `b`.

## Example

```qsharplet min = MinI(314, 271);  // 271```

## See Also

- [Microsoft.Quantum.MinD](xref:Microsoft.Quantum.MinD)
- [Microsoft.Quantum.MinL](xref:Microsoft.Quantum.MinL)