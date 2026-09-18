---
title: IProgressNotificationCallback.Notify
second_title: Aspose.Tasks for .NET API Reference
description: IProgressNotificationCallback method. Called during project longrunning operations to provide progress information
type: docs
weight: 10
url: /net/aspose.tasks/iprogressnotificationcallback/notify/
---
## IProgressNotificationCallback.Notify method

Called during project long-running operations to provide progress information.

```csharp
public void Notify(ProgressNotificationArgs args)
```

| Parameter | Type | Description |
| --- | --- | --- |
| args | ProgressNotificationArgs | A [`ProgressNotificationArgs`](../../progressnotificationargs/) object containing progress information for the current operation. |

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

* class [ProgressNotificationArgs](../../progressnotificationargs/)
* interface [IProgressNotificationCallback](../)
* namespace [Aspose.Tasks](../../iprogressnotificationcallback/)
* assembly [Aspose.Tasks](../../../)


