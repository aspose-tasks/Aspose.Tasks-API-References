---
title: "Prj.TimescaleFinish"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La data in cui termina la scala temporale nella visualizzazione."
type: docs
weight: 730
url: /it/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

La data in cui la scala temporale nella visualizzazione termina.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.TimescaleFinish.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


