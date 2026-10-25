---
title: "Tsk.SubprojectName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Исходное расположение подпроекта"
type: docs
weight: 1070
url: /ru/net/aspose.tasks/tsk/subprojectname/
---
## Tsk.SubprojectName field

Исходное расположение подпроекта.

```csharp
public static readonly Key<string, TaskKey> SubprojectName;
```

## Примеры

Показывает, как создать задачу подпроекта.

```csharp
var project = new Project(DataDir + "SubProjectTask.mpp");

// Добавить задачу
var task = project.RootTask.Children.Add("Task 1");

// Установка новой ссылки на подпроект
task.Set(Tsk.SubprojectName, DataDir + "subProject.mpp");

project.Save(OutDir + "CreateSubProjectTask_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


