---
title: "Project.DefaultWeekWorkingDays"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene l'istanza della classe WeekDayCollection che rappresenta una raccolta dei giorni lavorativi settimanali predefiniti del progetto e degli orari di lavoro."
type: docs
weight: 370
url: /it/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Ottiene l'istanza della classe [`WeekDayCollection`](../../weekdaycollection/) che rappresenta una raccolta dei giorni lavorativi settimanali predefiniti del progetto e degli orari di lavoro.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Valore di ritorno

L'istanza della classe [`WeekDayCollection`](../../weekdaycollection/) che contiene un elenco di oggetti [`WeekDay`](../../weekday/).

## Osservazioni

I dati sono contenuti solo nei file mpp (non in xml).

## Esempi

Mostra come ottenere il giorno lavorativo settimanale predefinito.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### Vedi anche

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


