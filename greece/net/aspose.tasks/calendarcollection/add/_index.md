---
title: "CalendarCollection.Add"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος CalendarCollection. Προσθέτει ένα νέο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο"
type: docs
weight: 20
url: /el/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Προσθέτει ένα νέο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο.

```csharp
public Calendar Add(string name)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Όνομα ημερολογίου. |

### Τιμή Επιστροφής

Προστέθηκε το αντικείμενο [`Calendar`](../../calendar/).

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Προκαλείται όταν το όνομα του ημερολογίου είναι null. |

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε ένα τυπικό ημερολόγιο.

```csharp
var project = new Project();

// Ορίστε ένα ημερολόγιο και κάντε το τυπικό
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Προσθέτει ένα νέο ημερολόγιο με το καθορισμένο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Καθορισμένο όνομα. |
| baseCalendar | Calendar | Καθορισμένο βασικό ημερολόγιο. |

### Τιμή Επιστροφής

Προστέθηκε το αντικείμενο [`Calendar`](../../calendar/).

## Παραδείγματα

Δείχνει πώς να προσθέσετε νέα ημερολόγια.

```csharp
var project = new Project();

// Νέα ημερολόγια μπορούν να προστεθούν στη συλλογή ημερολογίων ενός έργου χρησιμοποιώντας τις υπερφορτώσεις Add της συλλογής.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Δείτε επίσης

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


