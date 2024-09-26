---
title: Project.DisplayOptions
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets an instance of the ProjectDisplayOptions class
type: docs
weight: 380
url: /net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Gets an instance of the [`ProjectDisplayOptions`](../../projectdisplayoptions/) class.

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Examples

Shows how to tune project's display options.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Set a value indicating whether to show warnings when Project identifies a possible scheduling conflict with a manually scheduled task.
// This option is available for Project 2010 version and later.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### See Also

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


