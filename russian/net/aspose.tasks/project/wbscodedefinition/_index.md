---
title: "Project.WBSCodeDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает или задает определение WBS Code Definition для проекта"
type: docs
weight: 1030
url: /ru/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

Получает или задает определение кода WBS для проекта.

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## Примеры

Показывает, как добавить коды WBS.

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

### См. также

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


