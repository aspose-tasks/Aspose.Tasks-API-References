---
title: Calendar
second_title: Aspose.Tasks για Αναφορά API .NET
description: Αντιπροσωπεύει ένα ημερολόγιο που χρησιμοποιείται σε ένα έργο.
type: docs
weight: 230
url: /el/net/aspose.tasks/calendar/
---
## Calendar class

Αντιπροσωπεύει ένα ημερολόγιο που χρησιμοποιείται σε ένα έργο.

```csharp
public class Calendar
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Λαμβάνει ή ορίζει το βασικό ημερολόγιο από το οποίο εξαρτάται αυτό το ημερολόγιο. Ισχύει μόνο εάν το ημερολόγιο δεν είναι βασικό ημερολόγιο. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Λαμβάνει αντικείμενο CalendarExceptionCollection. Η συλλογή εξαιρέσεων που σχετίζεται με το ημερολόγιο. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι βασικό ημερολόγιο. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι ημερολόγιο βάσης. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Λαμβάνει ή ορίζει το όνομα του ημερολογίου. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Λαμβάνει ή ορίζει το μοναδικό αναγνωριστικό του ημερολογίου. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Λήψη WeekDaysCollection για αυτό το ημερολόγιο. Η συλλογή των καθημερινών που καθορίζει το ημερολόγιο. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Λαμβάνει αντικείμενο WorkWeekCollections. Η συλλογή των εβδομάδων εργασίας που σχετίζεται με το ημερολόγιο. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Καθιστά ένα δεδομένο Ημερολόγιο ως 24ωρο Ημερολόγιο. Το Ημερολόγιο 24 ωρών είναι ένα Ημερολόγιο στο οποίο κάθε μέρα της εβδομάδας λειτουργεί με 24ωρες ώρες εργασίας. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Δημιουργεί ένα δεδομένο Ημερολόγιο ως Ημερολόγιο Νυχτερινής Βάρδιας. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Δημιουργεί προεπιλεγμένο τυπικό ημερολόγιο. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Αφαιρεί το ημερολόγιο από το έργο. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει ο καθορισμένος χρόνος εργασίας σύμφωνα με το ημερολόγιο. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει ο καθορισμένος χρόνος εργασίας σύμφωνα με το ημερολόγιο. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Επιστρέφει έναν κωδικό κατακερματισμού για την παρουσία της κλάσης. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας από την ημερομηνία. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Επιστρέφει Ημερομηνία Έναρξης με βάση την καθορισμένη Ημερομηνία λήξης και Διάρκεια. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Επιστρέφει Ημερομηνία Έναρξης με βάση την καθορισμένη Ημερομηνία λήξης και Διάρκεια. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Υπολογίζει την ημερομηνία και την ώρα λήξης της εργασίας από την ημερομηνία έναρξης, τα χωριστά μέρη και τη διάρκεια. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Επιστρέφει το ποσό των ωρών εργασίας κατά την ημερομηνία. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Ώρες εργασίας επιστροφής για τις καθορισμένες ημερομηνίες. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Επιστρέφει[`WorkingTimeCollection`](../workingtimecollection/) των ωρών εργασίας για την καθορισμένη ημερομηνία. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Καθορίζει εάν η ημέρα είναι εργάσιμη. |

### Παρατηρήσεις

Τα Τα ημερολόγια χρησιμοποιούνται για τον καθορισμό τυπικών ωρών εργασίας και μη. Τα έργα πρέπει να έχουν ένα βασικό ημερολόγιο. Οι εργασίες και οι πόροι μπορούν να έχουν τα δικά τους μη βασικά ημερολόγια που βασίζονται σε ένα βασικό ημερολόγιο.

### Παραδείγματα

Πώς να δημιουργήσετε απλό ημερολόγιο από την αρχή.

```csharp
[C#]
// δημιουργία κενού ημερολογίου
Calendar calendar = new Calendar("New calendar");
// προσθέτει προεπιλεγμένες εργάσιμες ημέρες (8 εργάσιμες ώρες από τις 9:00 έως τις 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// δημιουργία νέας νέας εργάσιμης ημέρας
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Ρυθμίζει το χρόνο εργασίας. Σημαντικό είναι μόνο μέρος του χρόνου του DateTime
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
' δημιουργία κενού ημερολογίου
Dim calendar As Calendar =  New Calendar("New calendar")
' προσθέτει προεπιλεγμένες εργάσιμες ημέρες (8 εργάσιμες ώρες από τις 9:00 έως τις 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' δημιουργία νέας νέας εργάσιμης ημέρας
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Ρυθμίζει το χρόνο εργασίας. Σημαντικό είναι μόνο μέρος του χρόνου του DateTime
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
' προσθέτει το Σαββατοκύριακο
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Tasks](../../aspose.tasks/)
* συνέλευση [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
