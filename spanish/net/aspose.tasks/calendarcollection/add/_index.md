---
title: "CalendarCollection.Add"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método CalendarCollection. Agrega un nuevo calendario base a este objeto CalendarCollection y devuelve el calendario agregado."
type: docs
weight: 20
url: /es/net/aspose.tasks/calendarcollection/add/
---
## Add(string) {#add}

Agrega un nuevo calendario base a este objeto CalendarCollection y devuelve el calendario agregado.

```csharp
public Calendar Add(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | Nombre del calendario. |

### Valor devuelto

Objeto [`Calendar`](../../calendar/) añadido.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Lanzado cuando el nombre del calendario es nulo. |

## Ejemplos

Muestra cómo crear un calendario estándar.

```csharp
var project = new Project();

// Define un calendario y hazlo estándar
var calendar = project.Calendars.Add("New Standard Calendar");
Calendar.MakeStandardCalendar(calendar);

project.Save(OutDir + "MakeAStandardCalendar_out.xml", SaveFileFormat.Xml);
```

### Ver también

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, Calendar) {#add_1}

Agrega un nuevo calendario con el calendario base especificado a este objeto CalendarCollection y devuelve el calendario agregado.

```csharp
public Calendar Add(string name, Calendar baseCalendar)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | Nombre especificado. |
| baseCalendar | Calendar | Calendario base especificado. |

### Valor devuelto

Objeto [`Calendar`](../../calendar/) añadido.

## Ejemplos

Muestra cómo agregar nuevos calendarios.

```csharp
var project = new Project();

// Se pueden agregar nuevos calendarios a la colección de calendarios de un proyecto usando las sobrecargas del método Add de la colección.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Ver también

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


