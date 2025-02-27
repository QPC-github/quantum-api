---
uid: Microsoft.Quantum.Diagnostics.EqualityFactR
title: EqualityFactR function
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Diagnostics
qsharp.name: EqualityFactR
qsharp.summary: Asserts that a classical Result variable has the expected value.
---

# EqualityFactR function

Namespace: [Microsoft.Quantum.Diagnostics](xref:Microsoft.Quantum.Diagnostics)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Asserts that a classical Result variable has the expected value.

```qsharp
function EqualityFactR (actual : Result, expected : Result, message : String) : Unit
```


## Input

### actual : [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal)

The variable to be checked.


### expected : [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal)

The expected value.


### message : [String](xref:microsoft.quantum.qsharp.valueliterals#string-literals)

Failure message string to be used when the assertion is triggered.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

