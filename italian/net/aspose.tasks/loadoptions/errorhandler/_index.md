---
title: "LoadOptions.ErrorHandler"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "LoadOptions proprietà. Ottiene o imposta un metodo di callback per gestire gli errori di parsing XML"
type: docs
weight: 40
url: /it/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Ottiene o imposta un metodo di callback per gestire gli errori di parsing XML.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Esempi

Mostra come leggere un progetto da un file XML Primavera con errori di analisi.

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

// Restituisce il progetto con UID speciale
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Mostra come caricare un progetto Primavera usando &lt;see cref="LoadOptions" /&gt; con gestione degli errori.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // imposta le opzioni di lettura Primavera
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // lavorare con il progetto...
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

### Vedi anche

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


