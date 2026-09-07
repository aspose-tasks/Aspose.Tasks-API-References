---
title: "ParseErrorArgs.FieldType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ParseErrorArgs. Λαμβάνει τον τύπο του πεδίου του αντικειμένου"
type: docs
weight: 30
url: /el/net/aspose.tasks/parseerrorargs/fieldtype/
---
## ParseErrorArgs.FieldType property

Λαμβάνει τον τύπο του πεδίου του αντικειμένου.

```csharp
public Type FieldType { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από ροή με αρχείο XML με μη έγκυρους χαρακτήρες.

```csharp
public static void LoadProjectFromFile(string pathToModifiedXml)
{
    // ανοίξτε το αρχείο που περιέχει XML με κατεστραμμένα χρονικά διαστήματα
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

### Δείτε επίσης

* class [ParseErrorArgs](../)
* namespace [Aspose.Tasks](../../parseerrorargs/)
* assembly [Aspose.Tasks](../../../)


