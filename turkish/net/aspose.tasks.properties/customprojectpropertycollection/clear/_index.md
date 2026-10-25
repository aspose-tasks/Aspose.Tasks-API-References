---
title: "CustomProjectPropertyCollection.Clear"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CustomProjectPropertyCollection yöntemi. PropertyCollection'ı temizler"
type: docs
weight: 40
url: /tr/net/aspose.tasks.properties/customprojectpropertycollection/clear/
---
## CustomProjectPropertyCollection.Clear method

PropertyCollection'ı temizler.

```csharp
public void Clear()
```

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

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


