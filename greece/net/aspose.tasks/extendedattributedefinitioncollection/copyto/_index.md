---
title: "ExtendedAttributeDefinitionCollection.CopyTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "ExtendedAttributeDefinitionCollection μέθοδος. Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τον καθορισμένο δείκτη του πίνακα"
type: docs
weight: 80
url: /el/net/aspose.tasks/extendedattributedefinitioncollection/copyto/
---
## ExtendedAttributeDefinitionCollection.CopyTo method

Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα.

```csharp
public void CopyTo(ExtendedAttributeDefinition[] array, int arrayIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | ExtendedAttributeDefinition[] | ο καθορισμένος μονοδιάστατος πίνακας για αντιγραφή των στοιχείων σε αυτόν |
| arrayIndex | Int32 | ο μηδενικός δείκτης του καθορισμένου πίνακα στον οποίο αρχίζει η αντιγραφή. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε συλλογές ορισμών εκτεταμένων χαρακτηριστικών.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // καθαρισμός εκτεταμένων ορισμών χαρακτηριστικών
        project.ExtendedAttributes.Clear();
    }
}

// δημιουργήστε ορισμό extended attribute για μια εργασία
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// εργασία με εκτεταμένους ορισμούς χαρακτηριστικών...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// εργασία με εκτεταμένους ορισμούς χαρακτηριστικών...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// εργασία με εκτεταμένους ορισμούς χαρακτηριστικών...

// αφαιρέστε extended attribute κατά δείκτη
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// χρησιμοποιήστε πρόσβαση δείκτη συλλογής
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// αντιγράψτε τα attributes σε άλλο project
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// αφαιρέστε όλους τους ορισμούς extended attribute
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### Δείτε επίσης

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttributeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../extendedattributedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


