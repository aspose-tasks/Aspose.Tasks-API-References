---
title: "Sınıf CustomProjectProperty"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Properties.CustomProjectProperty sınıfı. Özel bir özelliği temsil eder."
type: docs
weight: 1540
url: /tr/net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

Özel bir özelliği temsil eder.

```csharp
public sealed class CustomProjectProperty : Property
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Özelliğin adını alır. |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | Özelliğin tipini alır. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Özelliğin değerini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Özellik değerini dize olarak döndürür. |

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

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


