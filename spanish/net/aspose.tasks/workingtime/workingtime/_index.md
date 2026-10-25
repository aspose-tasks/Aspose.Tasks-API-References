---
title: "WorkingTime.WorkingTime"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor WorkingTime. Inicializa una nueva instancia de la clase WorkingTime con un intervalo con los tiempos de inicio y fin especificados"
type: docs
weight: 10
url: /es/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Inicializa una nueva instancia de la clase [`WorkingTime`](../) con un intervalo con los tiempos de inicio y fin especificados.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fromTime | DateTime | tiempo de inicio del intervalo |
| toTime | DateTime | tiempo de fin del intervalo |

## Ejemplos

Muestra cómo trabajar con información de tiempo de trabajo.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Estos datos tratan sobre el botón "Detalles." puedes establecer tiempos de trabajo especiales para un WeekDay especial o incluso marcarlo como no laborable.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Puedes recorrer más a fondo los tiempos de trabajo y mostrarlos.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### Ver también

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Inicializa una nueva instancia de la clase [`WorkingTime`](../) con un elemento de intervalo con los tiempos de inicio y fin especificados.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fromTime | TimeSpan | Tiempo de inicio del intervalo representado por la estructura TimeSpan. |
| toTime | TimeSpan | Tiempo de fin del intervalo representado por la estructura TimeSpan. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Cuando toTime es menor o igual al argumento toTime o cuando el intervalo entre fromTime y toTime es mayor de 24 horas. |

## Ejemplos

La sobrecarga del constructor de WorkingTime se puede usar para inicializar el inicio y el fin del intervalo usando TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Ver también

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Inicializa una nueva instancia de la clase [`WorkingTime`](../) con un elemento de intervalo con los tiempos de inicio y fin especificados.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fromHours | Int32 | Hora de inicio del intervalo representada por un número entero de horas (0-24). |
| toHours | Int32 | Hora de fin del intervalo representada por un número entero de horas (0-24). |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Cuando toTime es menor o igual al argumento toTime o cuando el intervalo entre fromTime y toTime es mayor de 24 horas. |

## Ejemplos

La sobrecarga del constructor de WorkingTime se puede usar para inicializar el inicio y el fin del intervalo usando horas completas:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Muestra cómo comprobar la igualdad del tiempo de trabajo.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// La igualdad de los calendarios se verifica contra las fechas de inicio y fin del tiempo de trabajo.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Ver también

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


