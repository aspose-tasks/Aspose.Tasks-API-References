---
title: "WeekDay.WeekDay"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor WeekDay. Inicializa una nueva instancia de la clase WeekDay con el tipo de día especificado"
type: docs
weight: 10
url: /es/net/aspose.tasks/weekday/weekday/
---
## WeekDay(DayType) {#constructor_1}

Inicializa una nueva instancia de la clase [`WeekDay`](../) con el tipo de día especificado.

```csharp
public WeekDay(DayType dayType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dayType | DayType | El tipo de día especificado. |

## Ejemplos

Muestra cómo crear un nuevo calendario definiendo los días de la semana.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");

// Agregar días laborables de lunes a jueves con horarios predeterminados
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// verifique las fechas de inicio y fin del día de excepción
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Establecer el viernes como día laborable corto

// Establece el tiempo laborable.
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// existe una forma de convertir <see cref=\"DayOfWeek\" /> a <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// imprimamos todos los tiempos de trabajo
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Ver también

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, IEnumerable&lt;WorkingTime&gt;) {#constructor_3}

Inicializa una nueva instancia de la clase [`WeekDay`](../) con el tipo de día especificado y la lista de períodos de trabajo.

```csharp
public WeekDay(DayType dayType, IEnumerable<WorkingTime> workingTimes)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dayType | DayType | El tipo de día especificado. |
| workingTimes | IEnumerable`1 | Lista de períodos de tiempo laborables. |

## Ejemplos

Muestra cómo crear un nuevo calendario definiendo los días de la semana.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");

// Agregar días laborables de lunes a jueves con horarios predeterminados
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// verifique las fechas de inicio y fin del día de excepción
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Establecer el viernes como día laborable corto

// Establece el tiempo laborable.
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// existe una forma de convertir <see cref=\"DayOfWeek\" /> a <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// imprimamos todos los tiempos de trabajo
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Ver también

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, params WorkingTime[]) {#constructor_2}

Inicializa una nueva instancia de la clase [`WeekDay`](../) con el tipo de día especificado y los períodos de trabajo.

```csharp
public WeekDay(DayType dayType, params WorkingTime[] workingTimes)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dayType | DayType | El tipo de día especificado. |
| workingTimes | WorkingTime[] | Arreglo de períodos de tiempo laborables. |

### Ver también

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay() {#constructor}

Inicializa una nueva instancia de la clase [`WeekDay`](../).

```csharp
public WeekDay()
```

## Ejemplos

Muestra cómo crear un nuevo calendario definiendo los días de la semana.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");

// Agregar días laborables de lunes a jueves con horarios predeterminados
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// verifique las fechas de inicio y fin del día de excepción
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Establecer el viernes como día laborable corto

// Establece el tiempo laborable.
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// existe una forma de convertir <see cref=\"DayOfWeek\" /> a <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// imprimamos todos los tiempos de trabajo
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Ver también

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


