---
title: "Класс GroupCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.GroupCollection. Содержит список объектов Group. Реализует интерфейс ICollectionGroup."
type: docs
weight: 780
url: /ru/net/aspose.tasks/groupcollection/
---
## GroupCollection class

Содержит список объектов [`Group`](../group/). Реализует интерфейс ICollection&lt;Group&gt;.

```csharp
public class GroupCollection : ICollection<Group>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Получает значение, указывающее, является ли эта коллекция только для чтения. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Преобразует коллекцию групп в список объектов [`Group`](../group/). |

## Примеры

Показывает, как работать с коллекцией групп.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// перебрать группы задач
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// перебрать группы ресурсов
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// очистить группы другого проекта
otherProject.TaskGroups.Clear();

// скопировать группы в другой проект
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// добавить пользовательскую группу задач
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// удалить все группы
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### См. также

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


