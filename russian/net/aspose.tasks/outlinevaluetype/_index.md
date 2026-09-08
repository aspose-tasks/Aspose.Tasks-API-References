---
title: "Перечисление OutlineValueType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.OutlineValueType. Указывает тип значения контура"
type: docs
weight: 1230
url: /ru/net/aspose.tasks/outlinevaluetype/
---
## OutlineValueType enumeration

Указывает тип значения структуры.

```csharp
public enum OutlineValueType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Null | `0` | Указывает тип нулевого значения контура. |
| Date | `1` | Указывает тип датового значения контура. |
| Duration | `2` | Указывает тип длительности значения контура. |
| Cost | `3` | Указывает тип стоимости значения контура. |
| Number | `4` | Указывает тип числового значения контура. |
| Flag | `5` | Указывает тип значения контура Flag. |
| Text | `6` | Указывает тип значения контура Text. |
| FinishDate | `7` | Указывает тип значения контура Finish Date. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


