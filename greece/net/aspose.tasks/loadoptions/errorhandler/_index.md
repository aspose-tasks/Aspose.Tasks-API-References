---
title: "LoadOptions.ErrorHandler"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "LoadOptions property. Λαμβάνει ή ορίζει μια μέθοδο callback για τη διαχείριση σφαλμάτων ανάλυσης xml"
type: docs
weight: 40
url: /el/net/aspose.tasks/loadoptions/errorhandler/
---
## LoadOptions.ErrorHandler property

Λαμβάνει ή ορίζει μια μέθοδο κλήσης για τη διαχείριση σφαλμάτων ανάλυσης XML.

```csharp
public ParseErrorCallback ErrorHandler { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο Primavera XML με σφάλμα ανάλυσης.

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

// Επιστρέφει έργο με ειδικό UID
var project = new Project(OutDir + "IgnoreInvalidCharacters_out.xml", loadOptions);
Console.WriteLine(project.Get(Prj.Name));
```

Δείχνει πώς να φορτώσετε ένα έργο Primavera χρησιμοποιώντας &lt;see cref="LoadOptions" /&gt; με διαχείριση σφαλμάτων.

```csharp
public void WorkWithLoadOptionsAndPrimaveraOptionsAndErrorHandler()
{
    var loadOptions = new LoadOptions();

    var primaveraOptions = new PrimaveraReadOptions
    {
        ProjectUid = 3882
    };

    // ορίστε επιλογές ανάγνωσης primavera
    loadOptions.PrimaveraReadOptions = primaveraOptions;
    loadOptions.ErrorHandler = CustomDurationHandlerForFile;

    var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);

    // εργαστείτε με το έργο...
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

### Δείτε επίσης

* delegate [ParseErrorCallback](../../parseerrorcallback/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


