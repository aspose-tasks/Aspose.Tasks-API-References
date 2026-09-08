---
title: "Project.WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt een WBS Code Definition op of stelt deze in voor het project"
type: docs
weight: 1030
url: /nl/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

Haalt de WBS-code-definitie voor het project op of stelt deze in.

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## Voorbeelden

Toont hoe WBS-codes toe te voegen.

```csharp
var project = new Project
{
    WBSCodeDefinition = new WBSCodeDefinition()
};
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask
{
    Length = 2,
    Separator = "-",
    Sequence = WBSSequence.OrderedNumbers
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask
{
    Length = 1,
    Separator = "-",
    Sequence = WBSSequence.OrderedUppercaseLetters
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


