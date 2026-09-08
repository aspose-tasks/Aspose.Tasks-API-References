---
title: "LoadOptions.ErrorHandler"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "LoadOptions eigenschap. Haalt een callback-methode op of stelt deze in om xml-parsefouten af te handelen"
type: docs
weight: 40
url: /nl/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Haalt een callback-methode op of stelt deze in om XML-parsefouten af te handelen.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Voorbeelden

Toont hoe een project te lezen uit een Primavera‑XML‑bestand met fouten bij het parseren.

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

// Retourneert project met speciale UID
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Toont hoe een Primavera-project te laden met &lt;see cref="LoadOptions" /&gt; met foutafhandeling.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // stel primavera-leesopties in
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // werken met het project...
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

### Zie ook

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


