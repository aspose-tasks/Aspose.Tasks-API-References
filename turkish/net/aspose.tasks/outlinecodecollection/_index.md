---
title: "Sınıf OutlineCodeCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OutlineCodeCollection sınıfı. OutlineCode nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 1160
url: /tr/net/aspose.tasks/outlinecodecollection/
---
## OutlineCodeCollection class

[`OutlineCode`](../outlinecode/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class OutlineCodeCollection : IList<OutlineCode>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodecollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/outlinecodecollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [Item](../../aspose.tasks/outlinecodecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodecollection/add/)(OutlineCode) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/outlinecodecollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/outlinecodecollection/contains/)(OutlineCode) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/outlinecodecollection/copyto/)(OutlineCode[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/outlinecodecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [IndexOf](../../aspose.tasks/outlinecodecollection/indexof/)(OutlineCode) | Bu koleksiyondaki belirtilen öğenin dizinini belirler. |
| [Insert](../../aspose.tasks/outlinecodecollection/insert/)(int, OutlineCode) | Belirtilen öğeyi belirtilen dizine ekler. |
| [Remove](../../aspose.tasks/outlinecodecollection/remove/)(OutlineCode) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [RemoveAt](../../aspose.tasks/outlinecodecollection/removeat/)(int) | Belirtilen dizindeki bir öğeyi kaldırır. |

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

* class [OutlineCode](../outlinecode/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


