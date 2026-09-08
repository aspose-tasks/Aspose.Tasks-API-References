---
title: "Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Определяет, должны ли ручные задачи оставаться на ближайшем рабочем времени, когда они становятся автоматически запланированными"
type: docs
weight: 400
url: /ru/net/aspose.tasks/prj/keeptaskonnearestworkingtimewhenmadeautoscheduled/
---
## Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled field

Определяет, должны ли ручные задачи сохраняться на ближайшее рабочее время при переводе в автоматическое планирование.

```csharp
public static readonly Key<NullableBool, PrjKey> KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled;
```

## Примеры

Показывает, как читать/записывать свойство Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled.

```csharp
var project = new Project();

project.Set(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled, true);

Console.WriteLine("Keep Task On Nearest Working Time When Made Auto Scheduled: " + project.Get(Prj.KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


