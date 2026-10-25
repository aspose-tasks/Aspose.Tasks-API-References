---
title: "Classe DayTypeCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.DayTypeCollection. Rappresenta una raccolta di oggetti DayType"
type: docs
weight: 460
url: /it/net/aspose.tasks/daytypecollection/
---
## DayTypeCollection class

Rappresenta una raccolta di oggetti [`DayType`](../daytype/).

```csharp
public class DayTypeCollection : IList<DayType>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/daytypecollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/daytypecollection/isreadonly/) { get; } | Restituisce un valore che indica se questa raccolta è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks/daytypecollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/daytypecollection/add/)(DayType) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/daytypecollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/daytypecollection/contains/)(DayType) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/daytypecollection/copyto/)(DayType[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/daytypecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/daytypecollection/indexof/)(DayType) | Determina l'indice dell'elemento specificato in questa collezione. |
| [Insert](../../aspose.tasks/daytypecollection/insert/)(int, DayType) | Inserisce l'elemento specificato all'indice specificato. |
| [Remove](../../aspose.tasks/daytypecollection/remove/)(DayType) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [RemoveAt](../../aspose.tasks/daytypecollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |

## Esempi

Mostra come utilizzare una raccolta di giorni della settimana per definire un'eccezione del calendario settimanale.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // elimina un tipo di giorno da "Exception 2" per tipo di giorno
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// elimina un tipo di giorno da "Exception 2" per indice
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Modifica le eccezioni (non ci sono eccezioni nei dati del progetto iniziale)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// rimuovi tutti i giorni della settimana per "Exception 3"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### Vedi anche

* enum [DayType](../daytype/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


