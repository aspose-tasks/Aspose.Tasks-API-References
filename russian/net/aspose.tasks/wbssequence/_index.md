---
title: "Перечисление WBSSequence"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.WBSSequence. Указывает последовательность для WBSCodeMask"
type: docs
weight: 3520
url: /ru/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

Указывает последовательность для WBSCodeMask

```csharp
public enum WBSSequence
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| OrderedNumbers | `0` | Указывает числовую последовательность WBS. |
| OrderedUppercaseLetters | `1` | Указывает последовательность WBS из заглавных букв. |
| OrderedLowercaseLetters | `2` | Указывает последовательность WBS из строчных букв. |
| UnorderedCharacters | `3` | Указывает неупорядоченную последовательность символов WBS. |

## Примеры

Показывает, как задать последовательности WBS.

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


