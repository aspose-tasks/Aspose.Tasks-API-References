---
title: "Класс WBSCodeMask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WBSCodeMask. Представляет маску кода WBS"
type: docs
weight: 3500
url: /ru/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

Представляет маску кода WBS.

```csharp
public class WBSCodeMask
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | Инициализирует новый экземпляр класса `WBSCodeMask`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Получает или задает количество символов в строке кода. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Получает уровень маски. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Получает или задает разделитель строки кода. Значение по умолчанию — Точка. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Получает или задает тип символа строки кода. |

## Примеры

Показывает, как создавать маски кода WBS.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


