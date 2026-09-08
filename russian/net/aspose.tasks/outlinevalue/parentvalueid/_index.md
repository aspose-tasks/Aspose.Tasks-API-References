---
title: "OutlineValue.ParentValueId"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство OutlineValue. Получает или задает Id родительского узла кода контура."
type: docs
weight: 50
url: /ru/net/aspose.tasks/outlinevalue/parentvalueid/
---
## OutlineValue.ParentValueId property

Получает или задает Id родительского узла кода контура.

```csharp
public int ParentValueId { get; set; }
```

## Примеры

Показывает, как работать с значениями контура.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// создать значение контура
var value = new OutlineValue();

// установить фактическое значение
value.Value = "Text value 1";

// установить уникальный Id значения кода контура в проекте
value.ValueId = 1;

// получить GUID, который идентифицирует это значение среди остальных в проекте
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// установить тип кода контура
value.Type = OutlineValueType.Text;

// установить описание значения контура
value.Description = "Text value descr 1";

// установить значение, указывающее, свернуто ли значение контура
value.IsCollapsed = false;

// проверить Id родительского значения
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// создать значение контура с длительностью
var value2 = new OutlineValue();

// установить значение длительности
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// установить уникальный Id значения кода контура в проекте
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### См. также

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)


