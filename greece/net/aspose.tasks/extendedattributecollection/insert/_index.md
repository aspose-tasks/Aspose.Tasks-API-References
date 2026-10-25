---
title: "ExtendedAttributeCollection.Insert"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ExtendedAttributeCollection. Εισάγει το καθορισμένο στοιχείο στη συγκεκριμένη θέση"
type: docs
weight: 100
url: /el/net/aspose.tasks/extendedattributecollection/insert/
---
## ExtendedAttributeCollection.Insert method

Εισάγει το καθορισμένο στοιχείο στον καθορισμένο δείκτη.

```csharp
public void Insert(int index, ExtendedAttribute item)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | Int32 | ο καθορισμένος μηδενικός δείκτης στον οποίο πρέπει να εισαχθεί το στοιχείο. |
| item | ExtendedAttribute | το καθορισμένο στοιχείο για εισαγωγή σε αυτή τη συλλογή. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε συλλογές extended attribute.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Λάβετε εργασία με δείκτη μηδέν
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // καθαρίστε τα extended attributes
    task.ExtendedAttributes.Clear();
}

// δημιουργήστε ορισμό extended attribute για μια εργασία
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// Προσθέστε extended attribute 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Προσθέστε extended attribute 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// εργαστείτε με extended attributes...

// αφαιρέστε extended attribute κατά δείκτη
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// χρησιμοποιήστε πρόσβαση δείκτη συλλογής
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// αντιγράψτε τα attributes σε άλλο project
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// αφαιρέστε όλους τους ορισμούς extended attribute
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### Δείτε επίσης

* class [ExtendedAttribute](../../extendedattribute/)
* class [ExtendedAttributeCollection](../)
* namespace [Aspose.Tasks](../../extendedattributecollection/)
* assembly [Aspose.Tasks](../../../)


