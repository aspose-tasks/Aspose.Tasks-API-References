---
title: "ExtendedAttribute.ToString"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ExtendedAttribute. Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς μιας εκτεταμένης ιδιότητας"
type: docs
weight: 110
url: /el/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς ενός επεκτατικού χαρακτηριστικού.

```csharp
public override string ToString()
```

### Τιμή Επιστροφής

Η αναπαράσταση συμβολοσειράς της εκτεταμένης ιδιότητας.

## Παραδείγματα

Δείχνει πώς να διαβάσετε εκτεταμένες ιδιότητες.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Ανάγνωση εκτεταμένων χαρακτηριστικών για εργασίες
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // διαβάστε κοινές πληροφορίες σχετικά με την εκτεταμένη ιδιότητα
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### Δείτε επίσης

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


