---
title: "OutlineValueCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος OutlineValueCollection. Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή"
type: docs
weight: 80
url: /el/net/aspose.tasks/outlinevaluecollection/getenumerator/
---
## OutlineValueCollection.GetEnumerator method

Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή.

```csharp
public IEnumerator<OutlineValue> GetEnumerator()
```

### Τιμή Επιστροφής

έναν απαριθμητή για αυτή τη συλλογή.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές τιμών περιγράμματος.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// καθαρισμός συλλογών τιμών
foreach (var outlineCode in project.OutlineCodes)
{
    // καθαρισμός μάσκων περιγράμματος
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// ενημέρωση τιμής μέσω πρόσβασης δείκτη
codeDefinition.Values[0].Value = "654321";

// επανάληψη πάνω από τιμές περιγράμματος
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// εργασία με τιμές περιγράμματος
// ...

// αφαίρεση τιμής όταν χρειάζεται
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// εισαγωγή τιμής στη θέση έναρξης
codeDefinition.Values.Insert(0, value);

// έλεγχος της θέσης της εισαχθείσας τιμής
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// εργασία με τιμές περιγράμματος
// ...

// αφαίρεση της τελευταίας τιμής από τη συλλογή
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// μπορεί κανείς να δημιουργήσει έναν άλλο ορισμό κώδικα περιγράμματος
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// και στη συνέχεια αντιγραφή τιμών περιγράμματος
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### Δείτε επίσης

* class [OutlineValue](../../outlinevalue/)
* class [OutlineValueCollection](../)
* namespace [Aspose.Tasks](../../outlinevaluecollection/)
* assembly [Aspose.Tasks](../../../)


