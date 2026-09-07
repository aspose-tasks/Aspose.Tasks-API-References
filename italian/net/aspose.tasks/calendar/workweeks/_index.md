---
title: "Calendar.WorkWeeks"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Ottiene l'oggetto WorkWeekCollections. La collezione di settimane lavorative associate al calendario."
type: docs
weight: 130
url: /it/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

Ottiene l'oggetto WorkWeekCollections. La raccolta delle settimane lavorative associate al calendario.

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## Esempi

Mostra come leggere le informazioni delle settimane lavorative.

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // Visualizza il nome della settimana lavorativa, le date di inizio e fine.
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // Questi dati riguardano il pulsante "Dettagli"; è possibile impostare orari di lavoro speciali per giorni della settimana specifici o persino renderli non lavorativi.
    foreach (var day in workWeek.WeekDays)
    {
        // Puoi inoltre attraversare gli orari di lavoro e visualizzarli.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### Vedi anche

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


