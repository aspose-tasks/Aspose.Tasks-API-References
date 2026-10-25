---
title: "Prj.DurationFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il formato per esprimere la durata complessiva"
type: docs
weight: 300
url: /it/net/aspose.tasks/prj/durationformat/
---
## Prj.DurationFormat field

Il formato per esprimere la durata complessiva.

```csharp
public static readonly Key<TimeUnitType, PrjKey> DurationFormat;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.DurationFormat.

```csharp
var project = new Project();

project.Set(Prj.DurationFormat, TimeUnitType.Day);

Console.WriteLine("Duration Format: " + project.Get(Prj.DurationFormat));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


