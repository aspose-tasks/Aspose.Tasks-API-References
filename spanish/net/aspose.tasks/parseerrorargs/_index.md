---
title: "Clase ParseErrorArgs"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ParseErrorArgs. Proporciona datos para el delegado ParseErrorCallback."
type: docs
weight: 1240
url: /es/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

Proporciona datos para el delegado [`ParseErrorCallback`](../parseerrorcallback/).

```csharp
public class ParseErrorArgs
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Obtiene la excepción generada durante el análisis del valor de cadena. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Obtiene el nombre del campo del objeto. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Obtiene el tipo del campo del objeto. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | Obtiene el valor de cadena que generó una excepción. |

## Ejemplos

Muestra cómo leer un proyecto desde un flujo con un archivo XML con caracteres no válidos.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // abre el archivo que contiene XML con intervalos de tiempo rotos
    var project = new Project(pathToModifiedXml, CustomDurationHandlerForFile2);
    Console.WriteLine(project.Get(Prj.Name));
}

public static object CustomDurationHandlerForFile2(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var newValue = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", newValue);
    return newValue;
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


