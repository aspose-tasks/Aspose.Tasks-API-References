---
title: "Aspose::Tasks::Calendar κλάση"
linktitle: "Ημερολόγιο"
articleTitle: "Ημερολόγιο"
second_title: "Aspose.Tasks για C++"
description: "Αντιπροσωπεύει ένα ημερολόγιο που χρησιμοποιείται σε ένα έργο."
type: docs
weight: 10
url: /el/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Αντιπροσωπεύει ένα ημερολόγιο που χρησιμοποιείται σε ένα έργο.

Πώς να δημιουργήσετε ένα απλό ημερολόγιο από την αρχή.

```cpp
[C#]
// Δημιουργία κενού ημερολογίου
Calendar calendar = new Calendar("New calendar");
// προσθέτει προεπιλεγμένες εργάσιμες ημέρες (8 εργάσιμες ώρες από 9:00 έως 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// Δημιουργία νέας εργάσιμης ημέρας
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Ορίζει τον χρόνο εργασίας. Μόνο το τμήμα ώρας του DateTime είναι σημαντικό.
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
// προσθέτει Σαββατοκύριακο
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```cpp
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

Τα ημερολόγια χρησιμοποιούνται για τον ορισμό τυπικών εργάσιμων και μη εργάσιμων ωρών. Τα έργα πρέπει να έχουν ένα βασικό ημερολόγιο. Οι εργασίες και οι πόροι μπορούν να έχουν τα δικά τους μη-βασικά ημερολόγια που βασίζονται σε ένα βασικό ημερολόγιο.

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Delete](./delete/) | Αφαιρεί το ημερολόγιο από το έργο. |
| [Equals](./equals/) | Επιστρέφει μια τιμή που υποδεικνύει εάν αυτό το αντίγραφο είναι ίσο με ένα καθορισμένο αντικείμενο. |
| [get_BaseCalendar](./get_basecalendar/) | Λαμβάνει το βασικό ημερολόγιο από το οποίο εξαρτάται αυτό το ημερολόγιο. Εφαρμόζεται μόνο εάν το ημερολόγιο δεν είναι βασικό ημερολόγιο. |
| [get_Exceptions](./get_exceptions/) | Λαμβάνει το αντικείμενο CalendarExceptionCollection. Η συλλογή των εξαιρέσεων που σχετίζονται με το ημερολόγιο. |
| [get_Guid](./get_guid/) | Λαμβάνει το Guid του ημερολογίου. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι βασικό ημερολόγιο. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Λαμβάνει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι ημερολόγιο βάσης. |
| [get_Name](./get_name/) | Λαμβάνει το όνομα του ημερολογίου. |
| [get_Uid](./get_uid/) | Λαμβάνει το μοναδικό αναγνωριστικό του ημερολογίου. |
| [get_WeekDays](./get_weekdays/) | Λαμβάνει το WeekDaysCollection για αυτό το ημερολόγιο. Η συλλογή των ημερών της εβδομάδας που ορίζει το ημερολόγιο. |
| [get_WorkWeeks](./get_workweeks/) | Λαμβάνει το αντικείμενο WorkWeekCollections. Η συλλογή των εργασιακών εβδομάδων που σχετίζονται με το ημερολόγιο. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Υπολογίζει την ημερομηνία κατά την οποία θα περάσει η καθορισμένη ποσότητα χρόνου εργασίας σύμφωνα με το ημερολόγιο. |
| [GetHashCode](./gethashcode/) | Επιστρέφει έναν κωδικό κατακερματισμού για το στιγμιότυπο της κλάσης. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Λαμβάνει το στιγμιότυπο ICalendar που μπορεί να χρησιμοποιηθεί για υπολογισμούς στην τομή των εργασιακών προγραμμάτων 2 ημερολογίων. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Υπολογίζει την έναρξη της επόμενης εργάσιμης ημέρας για την καθορισμένη ημερομηνία. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Υπολογίζει το τέλος της προηγούμενης εργάσιμης ημερομηνίας από την καθορισμένη ημερομηνία. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από την ημερομηνία έναρξής της, τα διαχωρισμένα μέρη και τη διάρκεια εργασίας. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Επιστρέφει την ποσότητα των εργάσιμων ωρών στην καθορισμένη ημερομηνία. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Επιστρέφει την ποσότητα των εργάσιμων ωρών μεταξύ των καθορισμένων ημερομηνιών. |
| [GetWorkingTimes](./getworkingtimes/) | Επιστρέφει το WorkingTimeCollection των εργάσιμων χρόνων για την καθορισμένη ημερομηνία. |
| [GetWorkStart](./getworkstart/) | Υπολογίζει την έναρξη του επόμενου εργάσιμου χρόνου ξεκινώντας από την καθορισμένη ημερομηνία και ώρα. |
| [IsDayWorking](./isdayworking/) | Καθορίζει εάν η καθορισμένη ημέρα είναι εργάσιμη ημέρα σύμφωνα με το ημερολόγιο. |
| [IsEmpty](./isempty/) | Επιστρέφει εάν το ημερολόγιο δεν έχει ορισμένες εργάσιμες ώρες. |
| [Make24HourCalendar](./make24hourcalendar/) | Μετατρέπει ένα δεδομένο Calendar σε 24Ωρο Calendar. Το 24Ωρο Calendar είναι ένα ημερολόγιο στο οποίο κάθε ημέρα της εβδομάδας λειτουργεί με συνεχείς ώρες εργασίας. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Μετατρέπει ένα δεδομένο Calendar σε Night Shift Calendar. |
| [MakeStandardCalendar](./makestandardcalendar/) | Δημιουργεί προεπιλεγμένο τυπικό ημερολόγιο. |
| [set_BaseCalendar](./set_basecalendar/) | Ορίζει το βασικό ημερολόγιο από το οποίο εξαρτάται αυτό το ημερολόγιο. Ισχύει μόνο εάν το ημερολόγιο δεν είναι βασικό ημερολόγιο. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Ορίζει μια τιμή που υποδεικνύει εάν το ημερολόγιο είναι ημερολόγιο βάσης. |
| [set_Name](./set_name/) | Ορίζει το όνομα του ημερολογίου. |
| [set_Uid](./set_uid/) | Ορίζει το μοναδικό αναγνωριστικό του ημερολογίου. |

