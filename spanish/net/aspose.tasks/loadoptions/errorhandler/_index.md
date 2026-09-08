---
title: "LoadOptions.ErrorHandler"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "LoadOptions propiedad. Obtiene o establece un método de devolución de llamada para manejar errores de análisis xml"
type: docs
weight: 40
url: /es/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Obtiene o establece un método de devolución de llamada para manejar errores de análisis XML.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Ejemplos

Muestra cómo leer un proyecto desde un archivo XML de Primavera con error de análisis.

```csharp
var options = new PrimaveraReadOptions
{
    ProjectUid = 4557
};

var loadOptions = new LoadOptions()
{
    PrimaveraReadOptions = options,
    ErrorHandler = CustomDurationHandlerForFile
};

// Devuelve el proyecto con UID especial.
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Muestra cómo cargar un proyecto Primavera usando &lt;see cref=\"LoadOptions\" /&gt; con manejo de errores.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // establecer opciones de lectura de primavera
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // trabajar con el proyecto...
}

private static object CustomDurationHandlerForFile(object sender, ParseErrorArgs args)
{
    var regex = new Regex("[*]{2}(\\d+)Hrs(\\d+)Mins(\\d+)Secs[*]{2}");
    if (args.FieldType != typeof(TimeSpan))
    {
        throw args.Exception;
    }

    Console.WriteLine("Object field: {0}, Object field type: {1}, Invalid value: {2}", args.FieldName, args.FieldType, args.InvalidValue);
    var duration = regex.Replace(args.InvalidValue, "PT$1H$2M$3S");
    var value = Duration.ParseTimeSpan(duration);
    Console.WriteLine("New value : {0}", value);
    return value;
}
```

### Ver también

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


