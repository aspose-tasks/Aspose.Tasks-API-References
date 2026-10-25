---
title: "OutlineCodeCollection.Clear"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "OutlineCodeCollection μέθοδος. Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή"
type: docs
weight: 50
url: /el/net/aspose.tasks/outlinecodecollection/clear/
---
## OutlineCodeCollection.Clear method

Αφαιρεί όλα τα στοιχεία από αυτή τη συλλογή.

```csharp
public void Clear()
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές outline code.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

for (var i = 0; i < collector.Tasks.Count; i++)
{
    var current = collector.Tasks[i];
    if (current.Get(Tsk.Id) == 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes for the " + current.Get(Tsk.Name) + " task.");
    Console.WriteLine("Count of outline codes: " + current.OutlineCodes.Count);
    foreach (var outlineCode in current.OutlineCodes)
    {
        Console.WriteLine("Field Id: " + outlineCode.FieldId);
        Console.WriteLine("Value Id: " + outlineCode.ValueId);
        Console.WriteLine("Value Guid: " + outlineCode.ValueGuid);
        Console.WriteLine();
    }
}

// προσθέστε έναν προσαρμοσμένο ορισμό outline code
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// δημιουργήστε outline code
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// μπορείτε να ελέγξετε ότι η συλλογή δεν είναι μόνο για ανάγνωση
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// εισαγάγετε κώδικα με 2 σε λάθος θέση
task.OutlineCodes.Insert(0, code2);

// διορθώστε το
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// εισαγάγετε κώδικα με 2 στη σωστή θέση
task.OutlineCodes.Insert(2, code2);

// ελέγξτε ότι ο κώδικας εισήχθη
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// εργαστείτε με outline codes
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// προσθέστε έναν προσαρμοσμένο ορισμό outline code
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// δημιουργήστε outline code
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// εργαστείτε με outline codes
// ...

// αφαιρέστε outline code
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// καθαρίστε όλες τις τιμές ταυτόχρονα
task.OutlineCodes.Clear();
```

### Δείτε επίσης

* class [OutlineCodeCollection](../)
* namespace [Aspose.Tasks](../../outlinecodecollection/)
* assembly [Aspose.Tasks](../../../)


