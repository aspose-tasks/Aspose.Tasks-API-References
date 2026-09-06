---
title: "WBSCodeMask.Length"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété WBSCodeMask. Obtient ou définit le nombre de caractères de la chaîne de code"
type: docs
weight: 20
url: /fr/net/aspose.tasks/wbscodemask/length/
---
## WBSCodeMask.Length property

Obtient ou définit le nombre de caractères de la chaîne de code.

```csharp
public byte Length { get; set; }
```

## Exemples

Montre comment créer des masques de code WBS.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

project.Recalculate();

Console.WriteLine("Number of WBS masks: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
var i = 0;
foreach (var cm in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("WBS Mask #{0}: Level->{1}", ++i, cm.Level);
}

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* class [WBSCodeMask](../)
* namespace [Aspose.Tasks](../../wbscodemask/)
* assembly [Aspose.Tasks](../../../)


