---
title: "Κλάση Calendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Calendar. Αντιπροσωπεύει ένα ημερολόγιο που χρησιμοποιείται σε ένα έργο."
type: docs
weight: 230
url: /el/net/aspose.tasks/calendar/
---
## Calendar class

Αντιπροσωπεύει ένα ημερολόγιο που χρησιμοποιείται σε ένα έργο.

```csharp
public class Calendar : ICalendar
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Λαμβάνει ή ορίζει το βασικό ημερολόγιο από το οποίο εξαρτάται αυτό το ημερολόγιο. Ισχύει μόνο εάν το ημερολόγιο δεν είναι βασικό ημερολόγιο. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Λαμβάνει το αντικείμενο CalendarExceptionCollection. Η συλλογή των εξαιρέσεων που σχετίζονται με το ημερολόγιο. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Λαμβάνει το Guid του ημερολογίου. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι βασικό ημερολόγιο. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι ημερολόγιο βάσης. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα του ημερολογίου. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Λαμβάνει ένα αντικείμενο που περιέχει ιδιότητες ειδικές για Primavera για ένα ημερολόγιο που διαβάζεται από μορφές Primavera. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό του ημερολογίου. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Λαμβάνει το WeekDaysCollection για αυτό το ημερολόγιο. Η συλλογή των εργάσιμων ημερών που ορίζει το ημερολόγιο. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Λαμβάνει το αντικείμενο WorkWeekCollections. Η συλλογή των εβδομάδων εργασίας που σχετίζονται με το ημερολόγιο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Κάνει ένα δεδομένο Calendar να είναι ένα 24Ωρο Calendar. Το 24Ωρο Calendar είναι ένα ημερολόγιο στο οποίο κάθε ημέρα της εβδομάδας λειτουργεί με αδιάλειπτες ώρες εργασίας. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Μετατρέπει ένα δεδομένο Ημερολόγιο σε Ημερολόγιο Νυχτερινής Βάρδιας. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Δημιουργεί προεπιλεγμένο τυπικό ημερολόγιο. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Αφαιρεί το ημερολόγιο από το έργο. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Επιστρέφει έναν κωδικό κατακερματισμού για το στιγμιότυπο της κλάσης. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας για την καθορισμένη ημερομηνία. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από την ημερομηνία έναρξής της, τα διαχωρισμένα μέρη και τη διάρκεια εργασίας. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Επιστρέφει την ποσότητα των εργάσιμων ωρών στην καθορισμένη ημερομηνία. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Επιστρέφει WorkUnit - Έναρξη, Λήξη και Διάρκεια των ωρών εργασίας για το καθορισμένο χρονικό διάστημα. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Επιστρέφει την ποσότητα των εργάσιμων ωρών μεταξύ των καθορισμένων ημερομηνιών. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Επιστρέφει το [`WorkingTimeCollection`](../workingtimecollection/) των ωρών εργασίας για την καθορισμένη ημερομηνία. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Υπολογίζει την έναρξη του επόμενου εργάσιμου χρόνου ξεκινώντας από την καθορισμένη ημερομηνία και ώρα. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Καθορίζει εάν η καθορισμένη ημέρα είναι εργάσιμη ημέρα σύμφωνα με το ημερολόγιο. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Επιστρέφει εάν το ημερολόγιο δεν έχει ορισμένες εργάσιμες ώρες. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | Λαμβάνει το στιγμιότυπο [`ICalendar`](../icalendar/) που μπορεί να χρησιμοποιηθεί για εκτέλεση υπολογισμών στην τομή των προγραμμάτων εργασίας δύο ημερολογίων. |

## Παρατηρήσεις

Τα ημερολόγια χρησιμοποιούνται για τον ορισμό τυπικών ωρών εργασίας και μη εργασίας. Τα έργα πρέπει να έχουν ένα βασικό ημερολόγιο. Οι εργασίες και οι πόροι μπορούν να έχουν τα δικά τους μη-βασικά ημερολόγια που βασίζονται σε ένα βασικό ημερολόγιο.

## Παραδείγματα

Πώς να δημιουργήσετε ένα απλό ημερολόγιο από το μηδέν.

```csharp
[C#]
// δημιουργήστε κενό ημερολόγιο
Calendar calendar = new Calendar("New calendar");
// προσθέτει προεπιλεγμένες εργάσιμες ημέρες (8 ώρες εργασίας από 9:00 έως 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// δημιουργήστε νέα εργάσιμη ημέρα
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Ορίζει χρόνο εργασίας. Μόνο το τμήμα ώρας του DateTime είναι σημαντικό.
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// προσθέτει το Σαββατοκύριακο
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

Δείχνει πώς να ορίσετε ένα νέο ημερολόγιο, να προσθέσετε ημέρες της εβδομάδας σε αυτό και να ορίσετε ώρες εργασίας για τις ημέρες.

```csharp
var project = new Project();

// Ορίστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// Προσθέστε εργάσιμες ημέρες από τη Δευτέρα έως την Πέμπτη με προεπιλεγμένα ωράρια
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Ορίστε την Παρασκευή ως σύντομη εργάσιμη ημέρα
var weekDay = new WeekDay(DayType.Friday);

// Ορίζει χρόνο εργασίας. Μόνο το τμήμα ώρας του DateTime είναι σημαντικό.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// εργασία με το έργο...
```

### Δείτε επίσης

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


