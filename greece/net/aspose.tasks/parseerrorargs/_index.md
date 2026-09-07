---
title: "Κλάση ParseErrorArgs"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.ParseErrorArgs κλάση. Παρέχει δεδομένα για τον delegate ParseErrorCallback"
type: docs
weight: 1240
url: /el/net/aspose.tasks/parseerrorargs/
---
## ParseErrorArgs class

Παρέχει δεδομένα για τον delegate [`ParseErrorCallback`](../parseerrorcallback/).

```csharp
public class ParseErrorArgs
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Exception](../../aspose.tasks/parseerrorargs/exception/) { get; } | Λαμβάνει την εξαίρεση που προέκυψε κατά την ανάλυση της τιμής της συμβολοσειράς. |
| [FieldName](../../aspose.tasks/parseerrorargs/fieldname/) { get; } | Λαμβάνει το όνομα του πεδίου του αντικειμένου. |
| [FieldType](../../aspose.tasks/parseerrorargs/fieldtype/) { get; } | Λαμβάνει τον τύπο του πεδίου του αντικειμένου. |
| [InvalidValue](../../aspose.tasks/parseerrorargs/invalidvalue/) { get; } | Λαμβάνει την τιμή της συμβολοσειράς που προκάλεσε εξαίρεση. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


