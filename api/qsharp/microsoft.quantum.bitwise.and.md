---
uid: Microsoft.Quantum.Bitwise.And
title: And function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Bitwise
qsharp.name: And
qsharp.summary: >-
  Returns the bitwise AND of two integers.
  This performs the same computation as the built-in `&&&` operator.
---

# And function

Namespace: [Microsoft.Quantum.Bitwise](xref:Microsoft.Quantum.Bitwise)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Returns the bitwise AND of two integers.This performs the same computation as the built-in `&&&` operator.

```qsharp
function And (a : Int, b : Int) : Int
```


## Input

### a : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)




### b : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)





## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)



## Example

```qsharplet a = 248;       //                11111000₂let b = 63;        //                00111111₂let x = And(a, b); // x : Int = 56 = 00111000₂.```

## Remarks

See the [C# &amp; Operator](https://docs.microsoft.com/dotnet/csharp/language-reference/operators/and-operator) (binary) for more details.