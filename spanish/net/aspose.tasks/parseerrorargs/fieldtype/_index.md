---
title: "ParseErrorArgs.FieldType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ParseErrorArgs. Obtiene el tipo de campo del objeto"
type: docs
weight: 30
url: /es/net/aspose.tasks/parseerrorargs/fieldtype/
---
## ParseErrorArgs.FieldType property

Obtiene el tipo del campo del objeto.

```csharp
public Type FieldType { get; }
```

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

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


