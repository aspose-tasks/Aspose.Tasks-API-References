---
title: "WeekDay.WeekDay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WeekDay constructor. Initialiseert een nieuw exemplaar van de WeekDay-klasse met het opgegeven dagtype"
type: docs
weight: 10
url: /nl/net/aspose.tasks/weekday/weekday/
---
## WeekDay(DayType) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`WeekDay`](../) klasse met het opgegeven dagtype.

```csharp
public WeekDay(DayType dayType)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dayType | DayType | Het opgegeven dagtype. |

## Voorbeelden

Toont hoe een nieuwe kalender te maken door weekdagen te definiëren.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// controleer van‑ en tot‑datums van de uitzonderingsdag
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Stel vrijdag in als korte werkdag

// Stelt werktijd in. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// er is een manier om <see cref=\"DayOfWeek\" /> te converteren naar <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// laten we alle werktijden afdrukken
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Zie ook

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, IEnumerable&lt;WorkingTime&gt;) {#constructor_3}

Initialiseert een nieuw exemplaar van de [`WeekDay`](../) klasse met het opgegeven dagtype en een lijst van werktijdperioden.

```csharp
public WeekDay(DayType dayType, IEnumerable<WorkingTime> workingTimes)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dayType | DayType | Het opgegeven dagtype. |
| workingTimes | IEnumerable`1 | Lijst van werktijdperioden. |

## Voorbeelden

Toont hoe een nieuwe kalender te maken door weekdagen te definiëren.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// controleer van‑ en tot‑datums van de uitzonderingsdag
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Stel vrijdag in als korte werkdag

// Stelt werktijd in. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// er is een manier om <see cref=\"DayOfWeek\" /> te converteren naar <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// laten we alle werktijden afdrukken
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Zie ook

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, params WorkingTime[]) {#constructor_2}

Initialiseert een nieuw exemplaar van de [`WeekDay`](../) klasse met het opgegeven dagtype en werktijdperioden.

```csharp
public WeekDay(DayType dayType, params WorkingTime[] workingTimes)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dayType | DayType | Het opgegeven dagtype. |
| workingTimes | WorkingTime[] | Array van werktijdperioden. |

### Zie ook

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay() {#constructor}

Initialiseert een nieuw exemplaar van de [`WeekDay`](../) klasse.

```csharp
public WeekDay()
```

## Voorbeelden

Toont hoe een nieuwe kalender te maken door weekdagen te definiëren.

```csharp
var project = new Project();

// Definieer een kalender
var calendar = project.Calendars.Add("Calendar1");

// Voeg werkdagen toe van maandag tot en met donderdag met standaardtijden
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// controleer van‑ en tot‑datums van de uitzonderingsdag
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Stel vrijdag in als korte werkdag

// Stelt werktijd in. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// er is een manier om <see cref=\"DayOfWeek\" /> te converteren naar <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// laten we alle werktijden afdrukken
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Zie ook

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


