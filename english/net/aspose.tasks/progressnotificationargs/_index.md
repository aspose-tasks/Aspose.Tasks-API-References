---
title: Class ProgressNotificationArgs
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ProgressNotificationArgs class. Provides data for the Notify method
type: docs
weight: 1430
url: /net/aspose.tasks/progressnotificationargs/
---
## ProgressNotificationArgs class

Provides data for the [`Notify`](../iprogressnotificationcallback/notify/) method.

```csharp
public sealed class ProgressNotificationArgs : EventArgs
```

## Properties

| Name | Description |
| --- | --- |
| [CurrentStepName](../../aspose.tasks/progressnotificationargs/currentstepname/) { get; } | Gets the name of the current step (part of the operation) being executed. |
| [CurrentStepProgress](../../aspose.tasks/progressnotificationargs/currentstepprogress/) { get; } | Gets the estimated progress percentage completed for the current step (part of the operation) (0-100). |
| [EstimatedTotalProgress](../../aspose.tasks/progressnotificationargs/estimatedtotalprogress/) { get; } | Gets the estimated total progress of the entire operation (0-100). |

## Remarks

This class contains progress information about the operation.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


