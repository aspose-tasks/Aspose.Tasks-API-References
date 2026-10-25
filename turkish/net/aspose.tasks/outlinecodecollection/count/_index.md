---
title: "OutlineCodeCollection.Count"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineCodeCollection özelliği. Bu koleksiyonda bulunan öğelerin sayısını alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/outlinecodecollection/count/
---
## OutlineCodeCollection.Count property

Bu koleksiyonda bulunan öğe sayısını alır.

```csharp
public int Count { get; }
```

## Örnekler

Outline kod koleksiyonlarıyla nasıl çalışılacağını gösterir.

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

// özel bir outline kod tanımı ekleyin
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// outline kodu oluşturun
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// koleksiyonun yalnızca okunur olmadığını kontrol edebilirsiniz
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// 2 ile kodu yanlış bir konuma ekleyin
task.OutlineCodes.Insert(0, code2);

// düzeltin
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// 2 ile kodu doğru bir konuma ekleyin
task.OutlineCodes.Insert(2, code2);

// kodun eklendiğini kontrol edin
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// outline kodlarıyla çalışın
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// özel bir outline kod tanımı ekleyin
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// outline kodu oluşturun
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// outline kodlarıyla çalışın
// ...

// outline kodunu kaldırın
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// tüm değerleri bir kerede temizleyin
task.OutlineCodes.Clear();
```

### Ayrıca Bakınız

* class [OutlineCodeCollection](../)
* namespace [Aspose.Tasks](../../outlinecodecollection/)
* assembly [Aspose.Tasks](../../../)


