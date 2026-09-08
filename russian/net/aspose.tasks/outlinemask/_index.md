---
title: "Класс OutlineMask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.OutlineMask. Представляет четыре элемента маски, определяющей формат кода структуры."
type: docs
weight: 1190
url: /ru/net/aspose.tasks/outlinemask/
---
## OutlineMask class

Представляет четыре элемента маски, определяющей формат кода структуры.

```csharp
public class OutlineMask
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [OutlineMask](outlinemask/)() | Инициализирует новый экземпляр класса `OutlineMask`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Получает или задает максимальную длину (в символах) значений кода структуры. 0, если длина не определена. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Получает или задает уровень маски. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Получает или задает разделитель кодовых значений. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Получает или задает тип маски. |

## Примеры

Показывает, как работать с масками структуры.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// задать тип маски
mask.Type = MaskType.Characters;

// задать разделитель кодовых значений
mask.Separator = "/";

// задать уровень маски
mask.Level = 1;

// задать максимальную длину (в символах) кодовых значений структуры. 0, если длина не определена.
mask.Length = 2;

// добавить маску в определение
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


