---
title: "Calendar.Exceptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene el objeto CalendarExceptionCollection. La colección de excepciones que está asociada con el calendario"
type: docs
weight: 50
url: /es/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Obtiene el objeto CalendarExceptionCollection. La colección de excepciones asociada al calendario.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Ejemplos

Muestra cómo recuperar información sobre las excepciones del calendario.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Iterar sobre los calendarios
foreach (var calendar in project.Calendars)
{
    // Acceder a las excepciones del calendario
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### Ver también

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


