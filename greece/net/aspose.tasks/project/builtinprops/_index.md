---
title: "Project.BuiltInProps"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει τη συλλογή ενσωματωμένων ιδιοτήτων του project"
type: docs
weight: 100
url: /el/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

Λαμβάνει τη συλλογή ενσωματωμένων ιδιοτήτων του έργου.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις μετα-ιδιότητες του έργου (παρωχημένο API).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// Οι προσαρμοσμένες ιδιότητες είναι διαθέσιμες μέσω της τυποποιημένης συλλογής
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// Οι ενσωματωμένες ιδιότητες είναι διαθέσιμες άμεσα
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// ή ως στοιχείο της συλλογής ενσωματωμένων ιδιοτήτων
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### Δείτε επίσης

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


