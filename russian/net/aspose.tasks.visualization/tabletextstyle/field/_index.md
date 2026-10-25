---
title: "TableTextStyle.Field"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TableTextStyle. Получает или задает поле, к которому применяется стиль. Field"
type: docs
weight: 20
url: /ru/net/aspose.tasks.visualization/tabletextstyle/field/
---
## TableTextStyle.Field property

Получает или задает поле, к которому применяется стиль. `Field`.

```csharp
public Field Field { get; set; }
```

## Примеры

Показывает, как настраивать стили текста таблицы, которые используются для оформления различных текстовых элементов в проекте.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// установить стиль текста первого названия задачи
var style1 = new TableTextStyle(1);
// установить поле, к которому будет применён стиль.
style1.Field = Field.TaskName;
// установить <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> стиля текста.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// установить размер шрифта стиля текста в пунктах.

// установить стиль текста второй продолжительности задачи
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // установить флаг, указывающий, что данные представления должны быть записаны
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### См. также

* enum [Field](../../../aspose.tasks/field/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


