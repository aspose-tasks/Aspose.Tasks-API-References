---
title: "Table.TableFields"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Table. Возвращает коллекцию TableFields, представляющую поля таблицы"
type: docs
weight: 90
url: /ru/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Получает коллекцию TableFields, представляющую поля таблицы.

```csharp
public TableFieldCollection TableFields { get; }
```

## Примеры

Показывает, как работать с таблицами проекта.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Определить новый пользовательский атрибут
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Добавить пользовательский текстовый атрибут к созданной задаче.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Настройте таблицу, добавив поле текстового атрибута
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### См. также

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


