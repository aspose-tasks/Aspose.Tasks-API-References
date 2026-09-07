---
title: "Rsc.RegularWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La quantità totale di lavoro non straordinario programmato da eseguire per la risorsa"
type: docs
weight: 570
url: /it/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

L'importo totale del lavoro non straordinario programmato da eseguire dalla risorsa.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


