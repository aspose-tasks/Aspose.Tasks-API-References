---
title: "Rsc.Work"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità totale di tempo programmato per una risorsa su un'attività"
type: docs
weight: 690
url: /it/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

L'importo totale di tempo programmato per una risorsa su un'attività.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


