---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Calcula la fecha en que pasará la cantidad especificada de tiempo de trabajo según el calendario"
type: docs
weight: 160
url: /es/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

Calcula la fecha en la que el tiempo de trabajo especificado habrá transcurrido según el calendario.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | Fecha de inicio. |
| trabajo | Duración | Duración del trabajo. |

### Valor devuelto

Fecha de finalización.

## Ejemplos

Muestra cómo calcular una fecha de finalización a partir de la fecha de inicio y el trabajo usando una instancia de calendario.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calcular fecha de finalización usando un calendario estándar
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Ver también

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

Calcula la fecha en la que el tiempo de trabajo especificado habrá transcurrido según el calendario.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| inicio | DateTime | Fecha de inicio. |
| trabajo | TimeSpan | Duración del trabajo. |

### Valor devuelto

Fecha de finalización.

## Ejemplos

Muestra cómo calcular una fecha de finalización a partir de la fecha de inicio y el trabajo (como un intervalo de tiempo) usando una instancia de calendario.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// calcular fecha de finalización usando un calendario estándar
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


