---
title: "Prj.DurationFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Формат выражения общей продолжительности"
type: docs
weight: 300
url: /ru/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

Формат представления общей продолжительности.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Примеры

Показывает, как читать/записывать свойство Prj.DurationFormat.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


