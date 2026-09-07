---
title: "Rsc.Calendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il calendario di una risorsa"
type: docs
weight: 190
url: /it/net/aspose.tasks/rsc/calendar/
---
## Rsc.Calendar field

Il calendario di una risorsa.

```csharp
public static readonly Key<Calendar, RscKey> Calendar;
```

## Esempi

Mostra come ottenere/impostare un calendario di risorsa.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var res = project.Resources.Add("Resource1");

// Aggiungi calendario standard e assegnalo alla risorsa
var cal = project.Calendars.Add("Resource1");
res.Set(Rsc.Calendar, cal);

// Visualizza il nome del calendario base per tutte le risorse
foreach (var resource in project.Resources)
{
    if (resource.Get(Rsc.Name) != null)
    {
        Console.WriteLine(resource.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


