---
title: "Κλάση CalendarCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η κλάση Aspose.Tasks.CalendarCollection. Αντιπροσωπεύει μια συλλογή αντικειμένων Calendar"
type: docs
weight: 240
url: /el/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Αντιπροσωπεύει μια συλλογή αντικειμένων [`Calendar`](../calendar/).

```csharp
public class CalendarCollection : IList<Calendar>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Λαμβάνει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `CalendarCollection`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Προσθέτει ένα νέο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Προσθέτει ένα νέο ημερολόγιο με το καθορισμένο βασικό ημερολόγιο σε αυτό το αντικείμενο CalendarCollection και επιστρέφει το προστιθέμενο ημερολόγιο. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Επιστρέφει ένα ημερολόγιο με το καθορισμένο όνομα. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Επιστρέφει ένα ημερολόγιο με το καθορισμένο UID. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Αφαιρεί το Calendar από τη συλλογή CalendarCollection του Project. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Μετατρέπει το αντικείμενο CalendarCollection σε λίστα αντικειμένων [`Calendar`](../calendar/). |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


