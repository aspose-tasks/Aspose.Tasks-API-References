---
title: "Delegado ParseErrorCallback"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Representa una devolución de llamada de método para manejar errores de análisis que pueden ocurrir al leer datos XML"
type: docs
weight: 1250
url: /es/net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

Representa una devolución de llamada de método para manejar errores de análisis que pueden ocurrir al leer datos XML.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | Objeto | el objeto origen del error de análisis. |
| args | ParseErrorArgs | la instancia de la clase [`ParseErrorArgs`](../parseerrorargs/) que contiene los datos del evento. |

### Valor devuelto

el valor forzado para establecer en el objeto remitente especificado.

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

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


