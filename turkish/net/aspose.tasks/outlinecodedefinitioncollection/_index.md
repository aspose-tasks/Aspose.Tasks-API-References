---
title: "OutlineCodeDefinitionCollection sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OutlineCodeDefinitionCollection sınıfı. OutlineCodeDefinition nesnelerinin bir koleksiyonunu temsil eder."
type: docs
weight: 1180
url: /tr/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

[`OutlineCodeDefinition`](../outlinecodedefinition/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Bu koleksiyondaki belirtilen öğenin dizinini belirler. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Belirtilen öğeyi belirtilen dizine ekler. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Belirtilen dizindeki bir öğeyi kaldırır. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Bu OutlineCodeDefinitionCollection nesnesini [`OutlineCodeDefinition`](../outlinecodedefinition/) nesnelerinin bir listesine dönüştürür. |

## Örnekler

Outline code definition koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// özel bir outline kod tanımı ekleyin
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // outline code definition'ı konuma ekle
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// outline code definition'ın indeksini bul
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// çizelge kodu tanımını düzenle
project.OutlineCodes[index].Alias = "New Alias";

// ...
// çizelge kodu tanımlarıyla çalış
// ...

// çizelge kodu tanımını kaldır
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// indeksine göre bir çizelge kodu tanımını kaldır
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// çizelge kodu tanımlarını kaldır
otherProject.OutlineCodes.Clear();

// çizelge kodu tanımlarını kopyala
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// çizelge kodu tanımlarıyla çalış
// ...

// çizelge kodu tanımlarını tek tek kaldır
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Ayrıca Bakınız

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


