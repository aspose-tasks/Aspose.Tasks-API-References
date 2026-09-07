---
title: "OutlineCodeDefinitionCollection.CopyTo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "OutlineCodeDefinitionCollection μέθοδος. Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα ξεκινώντας από τον καθορισμένο δείκτη πίνακα"
type: docs
weight: 70
url: /el/net/aspose.tasks/outlinecodedefinitioncollection/copyto/
---
## OutlineCodeDefinitionCollection.CopyTo method

Αντιγράφει τα στοιχεία αυτής της συλλογής στον καθορισμένο πίνακα, ξεκινώντας από τη συγκεκριμένη θέση του πίνακα.

```csharp
public void CopyTo(OutlineCodeDefinition[] array, int arrayIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | OutlineCodeDefinition[] | ο καθορισμένος μονοδιάστατος πίνακας για αντιγραφή των στοιχείων σε αυτόν |
| arrayIndex | Int32 | ο μηδενικός δείκτης του καθορισμένου πίνακα στον οποίο αρχίζει η αντιγραφή. |

## Παραδείγματα

Δείχνει πώς να εργάζεστε με συλλογές ορισμών κώδικα περιγράμματος.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// προσθέστε έναν προσαρμοσμένο ορισμό outline code
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // εισαγωγή ορισμού κώδικα περιγράμματος στη θέση
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// εύρεση του δείκτη του ορισμού κώδικα περιγράμματος
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// επεξεργαστείτε τον ορισμό κώδικα περιγράμματος
project.OutlineCodes[index].Alias = "New Alias";

// ...
// εργαστείτε με ορισμούς κώδικα περιγράμματος
// ...

// αφαιρέστε τον ορισμό κώδικα περιγράμματος
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// αφαιρέστε έναν ορισμό κώδικα περιγράμματος με βάση τον δείκτη
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// αφαιρέστε ορισμούς κώδικα περιγράμματος
otherProject.OutlineCodes.Clear();

// αντιγράψτε ορισμούς κώδικα περιγράμματος
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// εργαστείτε με ορισμούς κώδικα περιγράμματος
// ...

// αφαιρέστε ορισμούς κώδικα περιγράμματος ένας-ένας
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Δείτε επίσης

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


