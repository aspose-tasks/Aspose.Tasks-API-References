---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraReadOptions. Λαμβάνει ή ορίζει μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν"
type: docs
weight: 20
url: /el/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Λαμβάνει ή ορίζει μια σημαία που καθορίζει εάν τα αρχικά μοναδικά αναγνωριστικά των οντοτήτων πρέπει να διατηρηθούν.

```csharp
public bool PreserveUids { get; set; }
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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


