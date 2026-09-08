---
title: "Clase Value"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Value. Representa un valor en una lista de valores"
type: docs
weight: 2800
url: /es/net/aspose.tasks/value/
---
## Value class

Representa un valor en una lista de valores.

```csharp
public class Value
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Value](value/)() | Inicializa una nueva instancia de la clase `Value`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | Obtiene o establece el valor real si puede representarse como DateTime. El valor predeterminado es MinValue. |
| [Description](../../aspose.tasks/value/description/) { get; set; } | Obtiene o establece la descripción de un valor. |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | Obtiene o establece el valor real que se usa para representar Duration. |
| [Id](../../aspose.tasks/value/id/) { get; set; } | Obtiene o establece el identificador único de un valor en todo el proyecto. |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | Obtiene o establece el valor real que se usa para representar un número o valor de costo. |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | Obtiene o establece la información fonética sobre el nombre del campo personalizado. |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | Obtiene o establece el valor real que se usa para representar una cadena de texto. |
| [Val](../../aspose.tasks/value/val/) { get; set; } | Obtiene o establece el valor real en representación interna. Prefiera usar propiedades fuertemente tipadas que se enumeran a continuación. |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | Obtiene un GUID que identifica este valor entre los demás en todo el proyecto. |

## Ejemplos

Muestra cómo leer trabajo con valores de búsqueda.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Crear una definición de atributo extendido de tipo Texto
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Agregar valores de búsqueda para la definición de atributo extendido
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Crear una definición de atributo extendido de tipo Duración
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// Agregar valores de búsqueda para la definición de atributo extendido
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Crear una definición de atributo extendido de tipo Fecha
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Crear una definición de atributo extendido de tipo Número
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


