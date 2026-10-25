---
title: "Sınıf ExtendedAttributeCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ExtendedAttributeCollection sınıfı. ExtendedAttribute nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 530
url: /tr/net/aspose.tasks/extendedattributecollection/
---
## ExtendedAttributeCollection class

[`ExtendedAttribute`](../extendedattribute/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class ExtendedAttributeCollection : IList<ExtendedAttribute>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributecollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/extendedattributecollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [Item](../../aspose.tasks/extendedattributecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributecollection/add/)(ExtendedAttribute) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/extendedattributecollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/extendedattributecollection/contains/)(ExtendedAttribute) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/extendedattributecollection/copyto/)(ExtendedAttribute[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/extendedattributecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [IndexOf](../../aspose.tasks/extendedattributecollection/indexof/)(ExtendedAttribute) | Bu koleksiyondaki belirtilen öğenin dizinini belirler. |
| [Insert](../../aspose.tasks/extendedattributecollection/insert/)(int, ExtendedAttribute) | Belirtilen öğeyi belirtilen dizine ekler. |
| [Remove](../../aspose.tasks/extendedattributecollection/remove/)(ExtendedAttribute) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [RemoveAt](../../aspose.tasks/extendedattributecollection/removeat/)(int) | Belirtilen dizindeki bir öğeyi kaldırır. |

## Örnekler

Genişletilmiş öznitelik koleksiyonlarının nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Sıfır indeksli görevi al
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // genişletilmiş öznitelikleri temizle
    task.ExtendedAttributes.Clear();
}

// bir görev için genişletilmiş öznitelik tanımı oluştur
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

// Genişletilmiş öznitelik 1 ekle
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Genişletilmiş öznitelik 2 ekle
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// genişletilmiş özniteliklerle çalış...

// indeks ile genişletilmiş özniteliği kaldır
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// koleksiyon indeks erişimini kullan
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// öznitelikleri diğer projeye kopyala
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

// tüm genişletilmiş öznitelik tanımlarını kaldır
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### Ayrıca Bakınız

* class [ExtendedAttribute](../extendedattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


