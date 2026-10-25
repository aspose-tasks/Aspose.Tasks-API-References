---
title: "View.HighlightFilter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство View. Получает или задаёт значение, указывающее, выделяет ли Microsoft Project фильтр для единственного представления"
type: docs
weight: 40
url: /ru/net/aspose.tasks/view/highlightfilter/
---
## View.HighlightFilter property

Получает или задает значение, указывающее, выделяет ли Microsoft Project фильтр для отдельного представления.

```csharp
public bool HighlightFilter { get; set; }
```

## Примеры

Показывает, как работать с представлениями MS Project.

```csharp
// создать пустой проект без представлений
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// создать стандартное представление диаграммы Ганта
View view = new GanttChartView();

// установить некоторые свойства представления
// установить значение, указывающее, отображает ли Microsoft Project имя отдельного представления в списках View или Other Views в ленте
view.ShowInMenu = true;
// установить значение, указывающее, выделяет ли Microsoft Project фильтр для отдельного представления
view.HighlightFilter = true;

// запись следующих свойств не поддерживается
// устанавливает фильтр, используемый в отдельном представлении
view.Filter = null;
// устанавливает группу отдельного представления
view.Group = null;
// устанавливает таблицу отдельного представления
view.Table = null;

// настроим некоторые параметры представления
// установить количество первых столбцов, печатаемых на всех страницах
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// установить значение, указывающее, печатать ли указанное количество первых столбцов на всех страницах
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// добавить представление в наш проект
project.Views.Add(view);

// Флаг WriteViewData следует использовать для сохранения изменений project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// проверим некоторые свойства недавно добавленного представления
// вывести уникальный идентификатор представления
Console.WriteLine("View Uid: " + view.Uid);
// вывести тип экрана для отдельного представления
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### См. также

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


