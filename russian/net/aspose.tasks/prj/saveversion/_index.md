---
title: "Prj.SaveVersion"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Версия Microsoft Office Project, из которой был сохранён файл проекта"
type: docs
weight: 620
url: /ru/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

Версия Microsoft Office Project, из которой был сохранён файл проекта.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
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


