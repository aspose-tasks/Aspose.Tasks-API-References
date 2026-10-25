---
title: "Classe CalendarCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.CalendarCollection. Rappresenta una raccolta di oggetti Calendar"
type: docs
weight: 240
url: /it/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Rappresenta una raccolta di oggetti [`Calendar`](../calendar/).

```csharp
public class CalendarCollection : IList<Calendar>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto `CalendarCollection`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Aggiunge un nuovo calendario di base a questo oggetto CalendarCollection e restituisce il calendario aggiunto. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Aggiunge un nuovo calendario con il calendario di base specificato a questo oggetto CalendarCollection e restituisce il calendario aggiunto. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Restituisce un calendario con il nome specificato. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Restituisce un calendario con l'UID specificato. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Rimuove il calendario dalla CalendarCollection del progetto. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Converte l'oggetto CalendarCollection in un elenco di oggetti [`Calendar`](../calendar/). |

## Esempi

Mostra come aggiungere nuovi calendari.

```csharp
var project = new Project();

// I nuovi calendari possono essere aggiunti alla raccolta di calendari di un progetto utilizzando le sovraccariche del metodo Add della raccolta.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Vedi anche

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


