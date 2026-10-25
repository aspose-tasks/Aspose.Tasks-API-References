---
title: "Table.TableFields"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Table ιδιότητα. Παίρνει μια συλλογή TableFields που αντιπροσωπεύει τα πεδία στον πίνακα."
type: docs
weight: 90
url: /el/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

Λαμβάνει μια συλλογή TableFields που αντιπροσωπεύει τα πεδία στον πίνακα.

```csharp
public TableFieldCollection TableFields { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τους πίνακες του έργου.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// Ορίστε νέο προσαρμοσμένο χαρακτηριστικό
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// Προσθέστε προσαρμοσμένο χαρακτηριστικό κειμένου στην δημιουργημένη εργασία.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// Προσαρμόστε τον πίνακα προσθέτοντας πεδίο χαρακτηριστικού κειμένου
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Δείτε επίσης

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


