---
title: Delegate ParseErrorCallback
second_title: Aspose.Tasks for .NET API Reference
description: Represents a method callback to handle parse errors that can happen when reading xml data
type: docs
weight: 1230
url: /net/aspose.tasks/parseerrorcallback/
---
## ParseErrorCallback delegate

Represents a method callback to handle parse errors that can happen when reading xml data.

```csharp
public delegate object ParseErrorCallback(object sender, ParseErrorArgs args);
```

| Parameter | Type | Description |
| --- | --- | --- |
| sender | Object | the source object of the parsing error. |
| args | ParseErrorArgs | the instance of the [`ParseErrorArgs`](../parseerrorargs/) class that contains the event data. |

### Return Value

the coerced value to set to the specified sender object.

## Examples

Shows how to read a project from a stream with XML file with invalid characters.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // open the file which contains XML with broken timespans
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

### See Also

* class [ParseErrorArgs](../parseerrorargs/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


