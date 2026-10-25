---
title: "Перечисление CustomFieldType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.CustomFieldType. Указывает тип пользовательского поля"
type: docs
weight: 380
url: /ru/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Указывает тип пользовательского поля.

```csharp
public enum CustomFieldType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Null | `0` | Указывает тип пользовательского поля Null. |
| Cost | `1` | Указывает тип пользовательского поля Cost. |
| Date | `2` | Указывает тип пользовательского поля Date. |
| Duration | `3` | Указывает тип пользовательского поля Duration. |
| Finish | `4` | Указывает тип пользовательского поля Finish. |
| Flag | `5` | Указывает тип пользовательского поля Flag. |
| Number | `6` | Указывает тип пользовательского поля Number. |
| Start | `7` | Указывает тип пользовательского поля Start. |
| Text | `8` | Указывает тип пользовательского поля Text. |
| OutlineCode | `9` | Указывает тип пользовательского поля Outline Code. |
| RBS | `10` | Указывает тип пользовательского поля RBS (Resource Breakdown Structure). |

## Примеры

Показывает, как использовать &lt;see cref=\"CustomFieldType\" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// работа с определениями...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


