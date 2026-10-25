---
title: "Project.DefaultView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Возвращает или задает представление проекта по умолчанию"
type: docs
weight: 360
url: /ru/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Получает или задает представление проекта по умолчанию.

```csharp
public View DefaultView { get; set; }
```

## Примеры

Показывает, как работать с представлением проекта по умолчанию.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Получить представление по умолчанию
UsageView view = (TaskUsageView)project.DefaultView;

// Столбец заголовка деталей не будет отображаться
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Отобразить столбец заголовка деталей
view.DisplayDetailsHeaderColumn = true;

// Повторять заголовок деталей во всех строках назначений
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

Показывает, как работать с представлением Project и добавить столбец в представление по умолчанию (которое отображается при открытии файла MPP в MS Project).

```csharp
// создать пустой проект без представлений
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Изменить представление по умолчанию (это представление диаграммы Ганта).
// Или вы можете выбрать представление по имени или через экран представлений, используя коллекцию project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Флаг WriteViewData следует использовать для сохранения изменений свойств представления.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

### См. также

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


