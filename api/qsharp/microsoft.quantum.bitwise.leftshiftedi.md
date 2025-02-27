---
uid: Microsoft.Quantum.Bitwise.LeftShiftedI
title: LeftShiftedI function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Bitwise
qsharp.name: LeftShiftedI
qsharp.summary: >-
  Shifts the bitwise representation of a number left by a given number of
  bits.
---

# LeftShiftedI function

Namespace: [Microsoft.Quantum.Bitwise](xref:Microsoft.Quantum.Bitwise)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Shifts the bitwise representation of a number left by a given number ofbits.

```qsharp
function LeftShiftedI (value : Int, amount : Int) : Int
```


## Input

### value : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number whose bitwise representation is to be shifted to the left(more significant).


### amount : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of bits by which `value` is to be shifted to the left.



## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The value of `value`, shifted left by `amount` bits.

## Remarks

The following are equivalent:```qsharplet c = a <<< b;let c = LeftShiftedI(a, b);```