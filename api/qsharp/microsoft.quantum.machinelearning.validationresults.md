---
uid: Microsoft.Quantum.MachineLearning.ValidationResults
title: ValidationResults user defined type
ms.date: 6/5/2023 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: udt
qsharp.namespace: Microsoft.Quantum.MachineLearning
qsharp.name: ValidationResults
qsharp.summary: >-
  The results from having validated a classifier against a set of
  samples.
---

# ValidationResults user defined type

Namespace: [Microsoft.Quantum.MachineLearning](xref:Microsoft.Quantum.MachineLearning)

Package: [Microsoft.Quantum.MachineLearning](https://nuget.org/packages/Microsoft.Quantum.MachineLearning)


The results from having validated a classifier against a set ofsamples.

```qsharp

newtype ValidationResults = (NMisclassifications : Int, NValidationSamples : Int);
```



## Named Items

### NMisclassifications : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of misclassifications observed during validation.
### NValidationSamples : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

