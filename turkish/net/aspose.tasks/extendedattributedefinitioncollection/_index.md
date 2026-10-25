---
title: "Sınıf ExtendedAttributeDefinitionCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ExtendedAttributeDefinitionCollection sınıfı. ExtendedAttributeDefinition nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 550
url: /tr/net/aspose.tasks/extendedattributedefinitioncollection/
---
## ExtendedAttributeDefinitionCollection class

[`ExtendedAttributeDefinition`](../extendedattributedefinition/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class ExtendedAttributeDefinitionCollection : IList<ExtendedAttributeDefinition>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributedefinitioncollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/extendedattributedefinitioncollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değeri alır. |
| [Item](../../aspose.tasks/extendedattributedefinitioncollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür veya ayarlar. |
| [ParentProject](../../aspose.tasks/extendedattributedefinitioncollection/parentproject/) { get; } | `ExtendedAttributeDefinitionCollection` örneği için bir üst proje alır. Bu koleksiyon için bir üst proje döndürür. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributedefinitioncollection/add/)(ExtendedAttributeDefinition) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/extendedattributedefinitioncollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/extendedattributedefinitioncollection/contains/)(ExtendedAttributeDefinition) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/extendedattributedefinitioncollection/copyto/)(ExtendedAttributeDefinition[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetById](../../aspose.tasks/extendedattributedefinitioncollection/getbyid/)(int) | Kimliğe göre bir genişletilmiş öznitelik tanımı döndürür |
| [GetEnumerator](../../aspose.tasks/extendedattributedefinitioncollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [IndexOf](../../aspose.tasks/extendedattributedefinitioncollection/indexof/)(ExtendedAttributeDefinition) | Bu koleksiyondaki belirtilen öğenin dizinini belirler. |
| [Insert](../../aspose.tasks/extendedattributedefinitioncollection/insert/)(int, ExtendedAttributeDefinition) | Belirtilen öğeyi belirtilen dizine ekler. |
| [Remove](../../aspose.tasks/extendedattributedefinitioncollection/remove/)(ExtendedAttributeDefinition) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [RemoveAt](../../aspose.tasks/extendedattributedefinitioncollection/removeat/)(int) | Belirtilen dizindeki bir öğeyi kaldırır. |
| [ToList](../../aspose.tasks/extendedattributedefinitioncollection/tolist/)() | Bu ExtendedAttributeDefinitionCollection nesnesini, [`ExtendedAttributeDefinition`](../extendedattributedefinition/) sınıfının örneklerini içeren bir listeye dönüştürür. |

## Örnekler

Genişletilmiş öznitelik tanımı koleksiyonlarını nasıl kullanacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // genişletilmiş öznitelik tanımlarını temizle
        project.ExtendedAttributes.Clear();
    }
}

// bir görev için genişletilmiş öznitelik tanımı oluştur
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

// genişletilmiş öznitelik tanımlarıyla çalış...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// genişletilmiş öznitelik tanımlarıyla çalış...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// genişletilmiş öznitelik tanımlarıyla çalış...

// indeks ile genişletilmiş özniteliği kaldır
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// koleksiyon indeks erişimini kullan
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// öznitelikleri diğer projeye kopyala
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

// tüm genişletilmiş öznitelik tanımlarını kaldır
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### Ayrıca Bakınız

* class [ExtendedAttributeDefinition](../extendedattributedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


