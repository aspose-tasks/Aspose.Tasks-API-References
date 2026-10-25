---
title: "Prj.TimescaleStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Дата, с которой начинается шкала времени в представлении."
type: docs
weight: 740
url: /ru/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

Дата, когда временная шкала в представлении начинается.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Примеры

Показывает, как установить дату начала шкалы времени, чтобы настроить дату, с которой должно начинаться представление.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


