---
title: '%azure.target (magic command)'
description: Sets or displays the active execution target for Q# job submission in
  an Azure Quantum workspace.
author: anjbur
uid: microsoft.quantum.iqsharp.magic-ref.azure.target
ms.author: anburton
ms.date: 06/05/2023
ms.topic: managed-reference
---

<!--
    NB: This file has been automatically generated from Microsoft.Quantum.IQSharp.AzureClient.dll,
        please do not manually edit it.

    [DEBUG] JSON source:
        {"Name": "%azure.target", "Documentation": {"Summary": "Sets or displays the active execution target for Q# job submission in an Azure Quantum workspace.", "Full": null, "Description": "\r\nThis magic command allows for specifying or displaying the execution target for Q# job submission\r\nin an Azure Quantum workspace.\r\n\r\nThe Azure Quantum workspace must have been previously initialized\r\nusing the [`%azure.connect` magic command](https://docs.microsoft.com/qsharp/api/iqsharp-magic/azure.connect)\r\nmagic command. The specified execution target must be available in the workspace and support execution of Q# programs.\r\n\r\n#### Optional parameters\r\n\r\n- The target ID to set as the active execution target for Q# job submission. If not specified,\r\nthe currently active execution target is displayed.\r\n\r\n#### Possible errors\r\n\r\n- `NotConnected`: Not connected to any Azure Quantum workspace.\r\n- `InvalidTarget`: The specified target is not enabled in this workspace. Please make sure the target name is valid and that the associated provider is added to your workspace. To add a provider to your quantum workspace in the Azure Portal, see https://aka.ms/AQ/Docs/AddProvider \r\n- `NoTarget`: No execution target has been configured for Azure Quantum job submission.\r\n\r\n#### Target capabilities\r\n\r\nWhen setting a target, the target capability is set to\r\nthe maximum capability level supported by the given\r\ntarget, such that all capabilities allowed by the target\r\nare allowed in subsequent Q# compilation functions and\r\noperations.\r\n\r\nYou can restrict target capability levels\r\nfurther by using\r\n`qsharp.azure.target_capability()`.\r\nThis may be useful, for instance, when comparing\r\nfunctionality between different targets.\r\n                ", "Remarks": null, "Examples": ["\r\nSets the current target for Q# job submission to `provider.qpu`:\r\n```\r\nIn []: %azure.target provider.qpu\r\nOut[]: Loading package Microsoft.Quantum.Providers.Provider and dependencies...\r\n        Active target is now provider.qpu\r\n        <detailed properties of active execution target>\r\n```\r\n                    ", "\r\nClears the current target information:\r\n```\r\nIn []: %azure.target --clear\r\n```\r\n                    ", "\r\nDisplays the current target and all available targets in the current Azure Quantum workspace:\r\n```\r\nIn []: %azure.target\r\nOut[]: Current execution target: provider.qpu\r\n        Available execution targets: provider.qpu, provider.simulator\r\n        <detailed properties of active execution target>\r\n```\r\n                    "], "SeeAlso": null}, "AssemblyName": "Microsoft.Quantum.IQSharp.AzureClient"}
-->

# `%azure.target`

## Summary

Sets or displays the active execution target for Q# job submission in an Azure Quantum workspace.

## Description

This magic command allows for specifying or displaying the execution target for Q# job submission
in an Azure Quantum workspace.

The Azure Quantum workspace must have been previously initialized
using the [`%azure.connect` magic command](https://docs.microsoft.com/qsharp/api/iqsharp-magic/azure.connect)
magic command. The specified execution target must be available in the workspace and support execution of Q# programs.

#### Optional parameters

- The target ID to set as the active execution target for Q# job submission. If not specified,
the currently active execution target is displayed.

#### Possible errors

- `NotConnected`: Not connected to any Azure Quantum workspace.
- `InvalidTarget`: The specified target is not enabled in this workspace. Please make sure the target name is valid and that the associated provider is added to your workspace. To add a provider to your quantum workspace in the Azure Portal, see https://aka.ms/AQ/Docs/AddProvider
- `NoTarget`: No execution target has been configured for Azure Quantum job submission.

#### Target capabilities

When setting a target, the target capability is set to
the maximum capability level supported by the given
target, such that all capabilities allowed by the target
are allowed in subsequent Q# compilation functions and
operations.

You can restrict target capability levels
further by using
`qsharp.azure.target_capability()`.
This may be useful, for instance, when comparing
functionality between different targets.

## Examples for `%azure.target`

### Example 1

Sets the current target for Q# job submission to `provider.qpu`:
```
In []: %azure.target provider.qpu
Out[]: Loading package Microsoft.Quantum.Providers.Provider and dependencies...
        Active target is now provider.qpu
        <detailed properties of active execution target>
```

### Example 2

Clears the current target information:
```
In []: %azure.target --clear
```

### Example 3

Displays the current target and all available targets in the current Azure Quantum workspace:
```
In []: %azure.target
Out[]: Current execution target: provider.qpu
        Available execution targets: provider.qpu, provider.simulator
        <detailed properties of active execution target>
```
