---
title: Class SaveTemplateOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.SaveTemplateOptions class. Allows to specify additional options when saving a project as a template
type: docs
weight: 2180
url: /net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Allows to specify additional options when saving a project as a template.

```csharp
public class SaveTemplateOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Gets or sets a value indicating whether all actual values from a project template should be removed. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Gets or sets a value indicating whether all baseline values from a project template should be removed. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Gets or sets a value indicating whether all fixed costs from a project template should be removed. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Gets or sets a value indicating whether resource rates from a project template should be removed. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


