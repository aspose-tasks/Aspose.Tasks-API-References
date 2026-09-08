---
title: "Класс ViewCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ViewCollection. Содержит список объектов View. Реализует интерфейс ICollectionView"
type: docs
weight: 2900
url: /ru/net/aspose.tasks/viewcollection/
---
## ViewCollection class

Содержит список объектов [`View`](../view/). Реализует интерфейс ICollection&lt;View&gt;.

```csharp
public class ViewCollection : ICollection<View>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Получает родителя объекта View. Только для чтения [`Project`](../project/). |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Ищет View с указанным именем и возвращает первое вхождение в коллекции. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Ищет View с указанным свойством Screen и возвращает первое вхождение в коллекции. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Преобразует коллекцию представлений в список объектов [`View`](../view/). |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


