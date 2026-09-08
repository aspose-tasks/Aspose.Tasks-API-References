---
title: "Prj.TimescaleFinish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Дата завершения шкалы времени в представлении"
type: docs
weight: 730
url: /ru/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

Дата, когда временная шкала в представлении заканчивается.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Примеры

Показывает, как читать/записывать свойство Prj.TimescaleFinish.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


