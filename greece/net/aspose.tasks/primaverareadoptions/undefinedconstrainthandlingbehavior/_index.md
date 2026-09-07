---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PrimaveraReadOptions. Καθορίζει τη συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από τη μορφή XER"
type: docs
weight: 50
url: /el/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Καθορίζει τη συμπεριφορά που χρησιμοποιείται για την επεξεργασία εργασιών με ακαθόριστους περιορισμούς που διαβάζονται από μορφή XER.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


