---
title: "Enum BookingType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.BookingType. Specifica il tipo di prenotazione di una risorsa"
type: docs
weight: 150
url: /it/net/aspose.tasks/bookingtype/
---
## BookingType enumeration

Specifica il tipo di prenotazione di una risorsa.

```csharp
public enum BookingType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Undefined | `-1` | Indica che il valore non era definito nel file di progetto originale. |
| Committed | `0` | Indica il tipo di prenotazione Committed. |
| Proposed | `1` | Indica il tipo di prenotazione Proposed. |

## Osservazioni

Durante l'esportazione in XML i valori Undefined verranno eliminati dall'XML risultante.

## Esempi

Mostra come leggere/scrivere la proprietà Asn.BookingType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.BookingType, BookingType.Proposed);

Console.WriteLine("Booking Type: " + assignment.Get(Asn.BookingType));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


