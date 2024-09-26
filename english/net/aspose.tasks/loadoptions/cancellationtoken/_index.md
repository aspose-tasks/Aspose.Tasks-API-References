---
title: LoadOptions.CancellationToken
second_title: Aspose.Tasks for .NET API Reference
description: LoadOptions property. Gets or sets a token which can be used to cancel a project loading operation
type: docs
weight: 20
url: /net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Gets or sets a token which can be used to cancel a project loading operation.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Examples

Shows how to pass CancellationToken to cancel long-running Project loading operation.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts can be passed to another thread where method cts.Cancel() can be called to cancel project loading operation.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


