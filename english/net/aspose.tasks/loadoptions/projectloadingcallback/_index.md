---
title: LoadOptions.ProjectLoadingCallback
second_title: Aspose.Tasks for .NET API Reference
description: LoadOptions property. Gets or sets the callback to be invoked during project loading operations. Currently supported for MPP and XER formats
type: docs
weight: 70
url: /net/aspose.tasks/loadoptions/projectloadingcallback/
---
## LoadOptions.ProjectLoadingCallback property

Gets or sets the callback to be invoked during project loading operations. Currently supported for MPP and XER formats.

```csharp
public IProgressNotificationCallback ProjectLoadingCallback { get; set; }
```

## Examples

Shows how to use progress notification callback when loading a project.

```csharp
var loadOptions = new LoadOptions
{
    // Set the callback to receive progress updates
    ProjectLoadingCallback = new ProgressNotificationCallbackImplementation()
};

// Load the project with progress notification
var project = new Project(DataDir + "Project.mpp", loadOptions);

Console.WriteLine("Project loaded successfully.");
```

### See Also

* interface [IProgressNotificationCallback](../../iprogressnotificationcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


