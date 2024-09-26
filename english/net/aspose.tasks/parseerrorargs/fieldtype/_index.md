---
title: ParseErrorArgs.FieldType
second_title: Aspose.Tasks for .NET API Reference
description: ParseErrorArgs property. Gets the object field type
type: docs
weight: 30
url: /net/aspose.tasks/parseerrorargs/fieldtype/
---
## ParseErrorArgs.FieldType property

Gets the object field type.

```csharp
public Type FieldType { get; }
```

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

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


