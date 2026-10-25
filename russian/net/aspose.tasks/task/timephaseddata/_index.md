---
title: "Task.TimephasedData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает или задает объект TimephasedDataCollection этой задачи. Блок данных, разбитых по времени, связанный с задачей"
type: docs
weight: 1220
url: /ru/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Получает или задает объект TimephasedDataCollection этой задачи. Блок данных, распределенных по времени, связанный с задачей.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Примечания

Чтение поддерживается только для формата XML.

## Примеры

Показывает, как выполнить итерацию по timephased data задачи.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


