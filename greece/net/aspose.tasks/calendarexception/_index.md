---
title: "Κλάση CalendarException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.CalendarException. Αντιπροσωπεύει εξαιρετικές χρονικές περιόδους σε ένα ημερολόγιο."
type: docs
weight: 250
url: /el/net/aspose.tasks/calendarexception/
---
## CalendarException class

Αντιπροσωπεύει εξαιρετικές χρονικές περιόδους σε ένα ημερολόγιο.

```csharp
public sealed class CalendarException
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CalendarException](calendarexception/)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `CalendarException`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Λαμβάνει το DayTypeCollection για αυτό το αντικείμενο. Οι ημέρες της εβδομάδας στις οποίες η εξαίρεση είναι έγκυρη. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η καθορισμένη ημερομηνία ή τύπος ημέρας είναι εργάσιμη. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η περιοχή επανάληψης ορίζεται με την εισαγωγή αριθμού επαναλήψεων. False υποδεικνύει ότι η περιοχή επανάληψης ορίζεται με την εισαγωγή ημερομηνίας λήξης. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Λαμβάνει ή ορίζει την έναρξη του χρόνου της εξαίρεσης. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Λαμβάνει ή ορίζει το μήνα για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Λαμβάνει ή ορίζει την ημέρα του μήνα στην οποία προγραμματίζεται η επανάληψη της εξαίρεσης. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Λαμβάνει ή ορίζει το στοιχείο μήνα για τον οποίο προγραμματίζεται η επανάληψη της εξαίρεσης. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Λαμβάνει ή ορίζει τη θέση του στοιχείου μήνα μέσα σε ένα μήνα. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα της εξαίρεσης. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των επαναλήψεων για τις οποίες η εξαίρεση του ημερολογίου είναι έγκυρη. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Λαμβάνει το γονικό ημερολόγιο για αυτό το αντικείμενο. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Λαμβάνει ή ορίζει την περίοδο επανάληψης για την εξαίρεση. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Λαμβάνει ή ορίζει το τέλος του χρόνου της εξαίρεσης. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο της εξαίρεσης. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Λαμβάνει ή ορίζει το αντικείμενο WorkingTimeCollection. Η συλλογή των ωρών εργασίας που ορίζει τον χρόνο εργασίας κατά τη διάρκεια της εβδομάδας. Πρέπει να υπάρχει τουλάχιστον μία ώρα εργασίας και δεν μπορούν να υπάρχουν περισσότερες από πέντε. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Επιστρέφει true εάν η καθορισμένη παρουσία της δομής DateTime είναι η ημέρα εξαίρεσης. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Διαγράφει την παρουσία Exception από το αντικείμενο CalendarExceptionCollection του γονικού ημερολογίου. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Επιστρέφει τις ημερομηνίες στις οποίες η εξαίρεση του ημερολογίου είναι εφαρμόσιμη. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Επιστρέφει τον χρόνο εργασίας για μια εξαίρεση ημερολογίου. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε/αφαιρέσετε εξαιρέσεις ημερολογίου.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// δημιουργήστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// Δημιουργήστε εξαίρεση ημερών της εβδομάδας για μια αργία.
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// Ελέγξτε αν η ημερομηνία είναι εξαιρετική.
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// Αφαιρέστε μια εξαίρεση.
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// Προσθέστε μια εξαίρεση.
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// Εκτυπώστε τις εξαιρέσεις.
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


