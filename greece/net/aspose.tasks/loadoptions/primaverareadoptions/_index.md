---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "LoadOptions property. Λαμβάνει ή ορίζει μια καθορισμένη παρουσία της κλάσης PrimaveraReadOptions που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera, Primavera P6 XER ή Primavera P6 Xml"
type: docs
weight: 60
url: /el/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Λαμβάνει ή ορίζει μια καθορισμένη παρουσία της κλάσης [`PrimaveraReadOptions`](../../primaverareadoptions/) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera (Primavera P6 XER ή Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
```

## Παραδείγματα

Δείχνει πώς να φορτώσετε ένα έργο Primavera με το καθορισμένο Id χρησιμοποιώντας &lt;see cref=\"LoadOptions\" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// ορίστε τις επιλογές ανάγνωσης Primavera
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// εργαστείτε με το έργο...
```

### Δείτε επίσης

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


