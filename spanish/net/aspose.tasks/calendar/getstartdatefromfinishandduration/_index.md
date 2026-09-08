---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Devuelve la fecha de inicio basada en la fecha de finalización y duración especificadas"
type: docs
weight: 200
url: /es/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Devuelve la fecha de inicio basada en la fecha de finalización y la duración especificadas.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| finalizar | DateTime | La fecha de finalización especificada. |
| duración | Duración | La duración especificada. |

### Valor devuelto

Fecha de inicio calculada.

## Ejemplos

Muestra cómo obtener una fecha de inicio a partir de la fecha de finalización y la duración.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtener fecha de inicio a partir de la fecha de finalización y una duración
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 de abril de 2020 9:00 a.m. será impreso
Console.WriteLine(startDate);
```

### Ver también

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Devuelve la fecha de inicio basada en la fecha de finalización y la duración especificadas.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| finalizar | DateTime | La fecha de finalización especificada. |
| duración | TimeSpan | La duración especificada. |

### Valor devuelto

Fecha de inicio calculada.

## Ejemplos

Muestra cómo obtener una fecha de inicio a partir de la fecha de finalización y la duración (como un intervalo de tiempo).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtener fecha de inicio a partir de la fecha de finalización y una duración
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 de abril de 2020 9:00 a.m. será impreso
Console.WriteLine(startDate);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


