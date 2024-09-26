---
title: SaveTemplateOptions.RemoveBaselineValues
second_title: Aspose.Tasks for .NET API Reference
description: SaveTemplateOptions property. Gets or sets a value indicating whether all baseline values from a project template should be removed
type: docs
weight: 30
url: /net/aspose.tasks.saving/savetemplateoptions/removebaselinevalues/
---
## SaveTemplateOptions.RemoveBaselineValues property

Gets or sets a value indicating whether all baseline values from a project template should be removed.

```csharp
public bool RemoveBaselineValues { get; set; }
```

## Examples

Shows how to save project as a template by using options.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// create template save options
// and tune its properties
var options = new SaveTemplateOptions
{
    // set a value indicating whether all fixed costs from a project template should be removed
    RemoveFixedCosts = true,

    // set a value indicating whether all actual values from a project template should be removed
    RemoveActualValues = true,

    // set a value indicating whether resource rates from a project template should be removed
    RemoveResourceRates = true,

    // set a value indicating whether all baseline values from a project template should be removed
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### See Also

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


