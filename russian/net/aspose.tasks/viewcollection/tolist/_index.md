---
title: "ViewCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ViewCollection. Преобразует коллекцию представлений в список объектов View"
type: docs
weight: 120
url: /ru/net/aspose.tasks/viewcollection/tolist/
---
## ViewCollection.ToList method

Преобразует коллекцию представлений в список объектов [`View`](../../view/).

```csharp
public List<View> ToList()
```

### Возвращаемое значение

Обобщённый список объектов [`View`](../../view/).

## Примеры

Показывает, как работать с коллекциями представлений.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// преобразовать в простой список представлений
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// добавить новое представление
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// итерация по представлениям
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// удалить все представления сразу
project.Views.Clear();

// или по одному
{
    // подход 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // подход 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### См. также

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


