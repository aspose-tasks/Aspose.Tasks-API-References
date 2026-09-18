---
title: Interface IProgressNotificationCallback
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.IProgressNotificationCallback interface. Represents a callback interface for receiving notifications during longrunning project operations
type: docs
weight: 890
url: /net/aspose.tasks/iprogressnotificationcallback/
---
## IProgressNotificationCallback interface

Represents a callback interface for receiving notifications during long-running project operations.

```csharp
public interface IProgressNotificationCallback
```

## Methods

| Name | Description |
| --- | --- |
| [Notify](../../aspose.tasks/iprogressnotificationcallback/notify/)(ProgressNotificationArgs) | Called during project long-running operations to provide progress information. |

## Remarks

This interface allows clients to receive progress updates. Implement this interface to track the operation progress.

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


