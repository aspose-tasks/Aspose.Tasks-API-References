---
title: LoadOptions.ErrorHandler
second_title: Aspose.Tasks for .NET API Reference
description: LoadOptions property. Gets or sets a callback method to handle xml parse errors
type: docs
weight: 40
url: /net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Gets or sets a callback method to handle xml parse errors.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Examples

Shows how to read a project from a Primavera XML file with error parsing.

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

// Returns project with special Uid
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Shows how to load Primavera project using &lt;see cref="LoadOptions" /&gt; with error handling.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // set primavera reading options
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // work with the project...
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

### See Also

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


