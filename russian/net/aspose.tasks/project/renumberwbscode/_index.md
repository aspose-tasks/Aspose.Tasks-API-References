---
title: "Project.RenumberWBSCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Перенумеровывает WBS-коды всех задач"
type: docs
weight: 1180
url: /ru/net/aspose.tasks/project/renumberwbscode/
---
## RenumberWBSCode() {#renumberwbscode}

Перенумеровывает код WBS всех задач.

```csharp
public void RenumberWBSCode()
```

## Примеры

Показывает, как перенумеровать WBS-коды задач.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

IEnumerable<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// вывод: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode();

Console.WriteLine("\nWBS codes after: ");

// вывод: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RenumberWBSCode(List&lt;int&gt;) {#renumberwbscode_1}

Перенумеровывает код WBS прошедших задач.

```csharp
public void RenumberWBSCode(List<int> taskIds)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| taskIds | List`1 | Идентификаторы задач для перенумерации WBS-кодов. |

## Примеры

Показывает, как перенумеровать WBS-коды выбранных задач.

```csharp
var project = new Project(DataDir + "RenumberExample.mpp");

var tasks = new List<Task>(project.RootTask.SelectAllChildTasks());

Console.WriteLine("WBS codes before: ");

// вывод: ""; "1"; "2"; "4"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}

project.RenumberWBSCode(new List<int> { 1, 2, 3 });

Console.WriteLine("\nWBS codes after: ");

// вывод: ""; "1"; "2"; "3"
foreach (var task in tasks)
{
    Console.WriteLine("\"" + task.Get(Tsk.WBS) + "\"" + "; ");
}
```

### См. также

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


