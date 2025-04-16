---
title: Class ParseErrorArgs
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ParseErrorArgs class. Provides data for the ParseErrorCallback delegate
type: docs
weight: 1230
url: /net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

Provides data for the [`ParseErrorCallback`](../parseerrorcallback/) delegate.

```csharp
public class ParseErrorArgs
```

## Properties

| Name | Description |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Gets the raised exception during parsing string value. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Gets the object field name. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Gets the object field type. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | Gets the string value which raised an exception. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


