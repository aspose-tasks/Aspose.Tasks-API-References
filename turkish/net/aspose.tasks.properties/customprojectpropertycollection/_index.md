---
title: "Sınıf CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Properties.CustomProjectPropertyCollection sınıfı. Özel proje özelliklerinin bir koleksiyonunu temsil eder."
type: docs
weight: 1550
url: /tr/net/aspose.tasks.properties/customprojectpropertycollection/
---
## CustomProjectPropertyCollection class

Özel proje özelliklerinin bir koleksiyonunu temsil eder.

```csharp
public sealed class CustomProjectPropertyCollection : PropertyKeyedCollection<CustomProjectProperty>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CustomProjectPropertyCollection](customprojectpropertycollection/)() | `CustomProjectPropertyCollection` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| override [IsReadOnly](../../aspose.tasks.properties/customprojectpropertycollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(CustomProjectProperty) |  |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add)(string, bool) | Yeni bir özel özellik oluşturur. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_2)(string, DateTime) | Yeni bir özel özellik oluşturur. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_1)(string, double) | Yeni bir özel özellik oluşturur. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_3)(string, string) | Yeni bir özel özellik oluşturur. |
| [Clear](../../aspose.tasks.properties/customprojectpropertycollection/clear/)() | PropertyCollection'ı temizler. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |
| [Remove](../../aspose.tasks.properties/customprojectpropertycollection/remove/)(string) | Belirtilen ada sahip bir özelliği koleksiyondan kaldırır. |

## Örnekler

Özel proje özelliği koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// Yeni özel özellikler ekleyelim.
// Koleksiyon Boolean, DateTime, Double, String türlerini destekler.
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// Özel özellikler tiplenmiş koleksiyon aracılığıyla kullanılabilir.
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// Bir özel özellik değerini al.
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// Özel özelliklerin adları üzerinde yinele.
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// Bir değer, string anahtar ile silinebilir.
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// veya koleksiyonu tamamen temizleyebilir
project.CustomProps.Clear();
```

### Ayrıca Bakınız

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [CustomProjectProperty](../customprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


