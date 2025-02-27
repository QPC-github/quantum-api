---
uid: Microsoft.Quantum.Bitwise.Xor
title: Xor function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Bitwise
qsharp.name: Xor
qsharp.summary: >-
  Returns the bitwise exclusive-OR (XOR) of two integers.
  This performs the same computation as the built-in `^^^` operator.
---

# Xor function

Namespace: [Microsoft.Quantum.Bitwise](xref:Microsoft.Quantum.Bitwise)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Returns the bitwise exclusive-OR (XOR) of two integers.This performs the same computation as the built-in `^^^` operator.

```qsharp
function Xor (a : Int, b : Int) : Int
```


## Input

### a : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)




### b : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)





## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)



## Example

```qsharplet a = 248;       //                 11111000₂let b = 63;        //                 00111111₂let x = Xor(a, b); // x : Int = 199 = 11000111₂.```

## Remarks

See the [C# ^ Operator](https://docs.microsoft.com/dotnet/csharp/language-reference/operators/xor-operator) for more details.