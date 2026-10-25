---
title: "Prj.TimescaleStart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. La data in cui inizia la scala temporale nella visualizzazione."
type: docs
weight: 740
url: /it/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

La data in cui la scala temporale nella visualizzazione inizia.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Esempi

Mostra come impostare la data di inizio della scala temporale per regolare la data in cui la visualizzazione dovrebbe iniziare.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


