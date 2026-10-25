---
title: "GroupCollection.CopyTo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод GroupCollection. Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива."
type: docs
weight: 60
url: /ru/net/aspose.tasks/groupcollection/copyto/
---
## GroupCollection.CopyTo method

Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива.

```csharp
public void CopyTo(Group[] array, int arrayIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| массив | Group[] | указанный одномерный массив, в который копировать элементы |
| arrayIndex | Int32 | нуль‑базовый индекс указанного массива, с которого начинается копирование. |

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

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


