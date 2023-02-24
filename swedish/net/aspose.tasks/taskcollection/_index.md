---
title: Class TaskCollection
second_title: Aspose.Tasks för .NET API-referens
description: Aspose.Tasks.TaskCollection klass. Representerar en samling avTask objekt.
type: docs
weight: 2100
url: /sv/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Representerar en samling av[`Task`](../task/) objekt.

```csharp
public class TaskCollection : IList<Task>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Hämtar antalet objekt som finns i TaskCollection. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Får ett värde som anger om denna samling är skrivskyddad. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Returnerar elementet vid det angivna indexet. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Hämtar det överordnade projektet för TaskCollection-objektet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Lägger till ny uppgift i projektuppgiftssamlingen på samma dispositionsnivå som den senaste uppgiften. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Infogar en ny uppgift före en uppgift med angivet ID och på samma dispositionsnivå. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Lägger till en ny uppgift i barnuppgiftssamlingen. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Lägg till den angivna uppgiften till instansen av`TaskCollection`class. Om ParentProject.CalculationMode är None ska användaren anropa Project.Recalculate() efter att ha använt den här metoden (Det kommer att omplanera alla projektuppgifter (start-/slutdatum, ställer in tidiga/sena datum) och beräkna de beroende fälten som slacks, work och kostnadsfält, id och dispositionsnivåer). Om ParentProject.CalculationMode är Manuell kommer metoden endast att beräkna uppgifts-id, dispositionsnivå och dispositionsnummer automatiskt. Om ParentProject.CalculationMode är Automatic omplanerar metoden alla projekts uppgifter automatiskt_x000. datum, sätter tidiga/sena datum, beräknar slacks, arbets- och kostnadsfält, räknar om id och dispositionsnivåer). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Lägger till en ny återkommande uppgift i samlingen av barnuppgifter. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Kontrollerar om samlingen innehåller specificerat föremål. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Returnerar en uppgift med det angivna ID vars förfader är överordnad uppgift för denna samling . |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Returnerar en uppgift med det angivna Uid vars förfader är överordnad uppgift för denna samling . |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Returnerar en uppräkning för denna samling. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Detta är stubbimplementeringen av ILists Insert -metod, som bara kastar NotSupportedException |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Detta är stubbimplementeringen av ICollections Remove -metod, som bara kastar NotSupportedException |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Konverterar TaskCollection-objektet till en lista med[`Task`](../task/) objekt. |

### Se även

* class [Task](../task/)
* namnutrymme [Aspose.Tasks](../../aspose.tasks/)
* hopsättning [Aspose.Tasks](../../)


