---
title: "Класс WBSCodeDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WBSCodeDefinition. Представляет определение кода WBS."
type: docs
weight: 3490
url: /ru/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Представляет определение кода WBS.

```csharp
public class WBSCodeDefinition
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | Инициализирует новый экземпляр класса `WBSCodeDefinition`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | Возвращает коллекцию объектов WBSCodeMask. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Возвращает или задает префикс кода проекта. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Возвращает или задает значение, указывающее, следует ли генерировать код WBS для новой задачи. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Возвращает или задает значение, указывающее, следует ли проверять уникальность новых кодов WBS. |

## Примеры

Показывает, как добавить маски кода WBS.

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

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


