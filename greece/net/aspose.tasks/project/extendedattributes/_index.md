---
title: "Project.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει το αντικείμενο ExtendedAttributeDefinitionCollection. Η συλλογή των ορισμών προσαρμοσμένων πεδίων εκτεταμένων χαρακτηριστικών που σχετίζονται με ένα έργο"
type: docs
weight: 410
url: /el/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

Αποκτά το αντικείμενο ExtendedAttributeDefinitionCollection. Η συλλογή των ορισμών επεκταμένων χαρακτηριστικών (προσαρμοσμένων πεδίων) που σχετίζονται με ένα έργο.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με εκτεταμένα χαρακτηριστικά.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// Εάν το προσαρμοσμένο πεδίο δεν υπάρχει στο Project, δημιουργήστε το
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// Δημιουργία εκτεταμένου χαρακτηριστικού από τον ορισμό
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// Προσθήκη εκτεταμένου χαρακτηριστικού στην εργασία
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


