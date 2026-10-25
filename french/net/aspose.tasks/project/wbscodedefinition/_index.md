---
title: "Project.WBSCodeDefinition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient ou définit la définition du code WBS pour le projet"
type: docs
weight: 1030
url: /fr/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

Obtient ou définit la définition du code WBS pour le projet.

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## Exemples

Montre comment ajouter des codes WBS.

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

### Voir aussi

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


