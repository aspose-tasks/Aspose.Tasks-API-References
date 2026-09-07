---
title: "OutlineCodeCollection.Insert"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "OutlineCodeCollection मेथड। निर्दिष्ट आइटम को निर्दिष्ट इंडेक्स पर सम्मिलित करता है।"
type: docs
weight: 100
url: /hi/net/aspose.tasks/outlinecodecollection/insert/
---
## OutlineCodeCollection.Insert method

निर्दिष्ट सूचकांक पर निर्दिष्ट आइटम डालता है।

```csharp
public void Insert(int index, OutlineCode item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| इंडेक्स | Int32 | वह निर्दिष्ट शून्य-आधारित इंडेक्स जहाँ आइटम को सम्मिलित किया जाना चाहिए। |
| आइटम | OutlineCode | इस संग्रह में सम्मिलित करने के लिए निर्दिष्ट आइटम। |

## उदाहरण

दिखाता है कि आउटलाइन कोड संग्रहों के साथ कैसे काम करें।

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

// एक कस्टम आउटलाइन कोड परिभाषा जोड़ें
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// आउटलाइन कोड बनाएं
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// जांच सकते हैं कि संग्रह केवल पढ़ने योग्य नहीं है
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// कोड को 2 के साथ गलत स्थिति में डालें
task.OutlineCodes.Insert(0, code2);

// इसे ठीक करें
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// कोड को 2 के साथ सही स्थिति में डालें
task.OutlineCodes.Insert(2, code2);

// जांचें कि कोड डाला गया था
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// आउटलाइन कोड्स के साथ काम करें
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// एक कस्टम आउटलाइन कोड परिभाषा जोड़ें
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// आउटलाइन कोड बनाएं
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// आउटलाइन कोड्स के साथ काम करें
// ...

// आउटलाइन कोड हटाएं
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// सभी मानों को एक साथ साफ़ करें
task.OutlineCodes.Clear();
```

### संबंधित देखें

* class [OutlineCode](../../outlinecode/)
* class [OutlineCodeCollection](../)
* namespace [Aspose.Tasks](../../outlinecodecollection/)
* assembly [Aspose.Tasks](../../../)


