---
title: "CalendarCollection.Add"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo CalendarCollection. Aggiunge un nuovo calendario base a questo oggetto CalendarCollection e restituisce il calendario aggiunto."
type: docs
weight: 20
url: /it/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Aggiunge un nuovo calendario di base a questo oggetto CalendarCollection e restituisce il calendario aggiunto.

```csharp
public Calendar Add(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | Stringa | Nome del calendario. |

### Valore di ritorno

Aggiunto oggetto [`Calendar`](../../calendar/).

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Generato quando il nome del calendario è null. |

## Esempi

Mostra come creare un calendario standard.

```csharp
var project = new Project();

// Definisci un calendario e rendilo standard
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Aggiunge un nuovo calendario con il calendario di base specificato a questo oggetto CalendarCollection e restituisce il calendario aggiunto.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | Stringa | Nome specificato. |
| baseCalendar | Calendar | Calendario base specificato. |

### Valore di ritorno

Aggiunto oggetto [`Calendar`](../../calendar/).

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

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


