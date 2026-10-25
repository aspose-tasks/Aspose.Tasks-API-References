---
title: "Sınıf BuiltInProjectPropertyCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Properties.BuiltInProjectPropertyCollection sınıfı. Yerleşik proje özelliklerinin bir koleksiyonunu temsil eder."
type: docs
weight: 1530
url: /tr/net/aspose.tasks.properties/builtinprojectpropertycollection/
---
## BuiltInProjectPropertyCollection class

Yerleşik proje özelliklerinin bir koleksiyonunu temsil eder.

```csharp
public sealed class BuiltInProjectPropertyCollection : 
    PropertyKeyedCollection<BuiltInProjectProperty>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Author](../../aspose.tasks.properties/builtinprojectpropertycollection/author/) { get; set; } | Projenin yazarını alır veya ayarlar. |
| [Category](../../aspose.tasks.properties/builtinprojectpropertycollection/category/) { get; set; } | Projenin kategorisini alır veya ayarlar. |
| [Comments](../../aspose.tasks.properties/builtinprojectpropertycollection/comments/) { get; set; } | Projenin yorumlarını alır veya ayarlar. |
| [Company](../../aspose.tasks.properties/builtinprojectpropertycollection/company/) { get; set; } | Projenin şirketini alır veya ayarlar. |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| [HyperlinkBase](../../aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/) { get; set; } | Projenin hiperlink temelini alır veya ayarlar. |
| override [IsReadOnly](../../aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Keywords](../../aspose.tasks.properties/builtinprojectpropertycollection/keywords/) { get; set; } | Projenin anahtar kelimelerini alır veya ayarlar. |
| [Manager](../../aspose.tasks.properties/builtinprojectpropertycollection/manager/) { get; set; } | Projenin yöneticisini alır veya ayarlar. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |
| [Subject](../../aspose.tasks.properties/builtinprojectpropertycollection/subject/) { get; set; } | Bir projenin konusunu alır veya ayarlar. |
| [Title](../../aspose.tasks.properties/builtinprojectpropertycollection/title/) { get; set; } | Bir projenin başlığını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(BuiltInProjectProperty) |  |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |

## Örnekler

Proje yerleşik özelliklerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// yerleşik özellik koleksiyonunda yineleme yap
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [BuiltInProjectProperty](../builtinprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


