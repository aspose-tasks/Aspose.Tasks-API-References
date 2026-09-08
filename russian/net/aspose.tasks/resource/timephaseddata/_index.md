---
title: "Resource.TimephasedData"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает или задает экземпляр класса TimephasedDataCollection для этого объекта"
type: docs
weight: 740
url: /ru/net/aspose.tasks/resource/timephaseddata/
---
## Resource.TimephasedData property

Получает или задает экземпляр класса [`TimephasedDataCollection`](../../timephaseddatacollection/) для этого объекта.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Примечания

Чтение поддерживается только для формата XML.

## Примеры

Показывает, как читать timephased данные ресурса.

```csharp
resource.Set(Rsc.Work, resource.ParentProject.GetWork(2));

project.SetBaseline(BaselineType.Baseline);

// перебирайте timephased данные ресурса
foreach (var td in resource.TimephasedData)
{
    Console.WriteLine(td.Start);
    Console.WriteLine(td.Finish);
}
```

### См. также

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


