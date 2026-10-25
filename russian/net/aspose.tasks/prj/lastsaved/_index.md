---
title: "Prj.LastSaved"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Дата последнего сохранения проекта. Сохранено в формате UTC в файлах mpp. Тип DateTime."
type: docs
weight: 440
url: /ru/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

Дата последнего сохранения проекта. Сохранено в формате UTC в файлах mpp. Тип DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
```

## Примеры

Показывает, как проверить версию сохранения проекта и дату сохранения.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Отобразить версию проекта
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


