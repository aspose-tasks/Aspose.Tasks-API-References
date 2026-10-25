---
title: "OutlineMask.Length"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство OutlineMask. Получает или задает максимальную длину в символах значений кода контура. 0, если длина не определена"
type: docs
weight: 20
url: /ru/net/aspose.tasks/outlinemask/length/
---
## OutlineMask.Length property

Получает или задает максимальную длину (в символах) значений кода структуры. 0, если длина не определена.

```csharp
public int Length { get; set; }
```

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

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)


