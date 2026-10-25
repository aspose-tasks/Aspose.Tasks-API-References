---
title: "Project.Get"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Возвращает значение, к которому свойство сопоставлено в этом контейнере"
type: docs
weight: 1080
url: /ru/net/aspose.tasks/project/get/
---
## Project.Get&lt;T&gt; method

Возвращает значение, к которому свойство сопоставлено в этом контейнере.

```csharp
public T Get<T>(Key<T, PrjKey> key)
```

| Параметр | Описание |
| --- | --- |
| T | тип сопоставленного значения. |
| key | указанный ключ свойства. [`Prj`](../../prj/) для получения ключа свойства. |

### Возвращаемое значение

значение, к которому свойство сопоставлено в этом контейнере.

## Примеры

Показывает, как проверить версию проекта.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Отобразить версию проекта
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


