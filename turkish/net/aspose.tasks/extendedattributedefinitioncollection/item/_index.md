---
title: "ExtendedAttributeDefinitionCollection.Item"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ExtendedAttributeDefinitionCollection özelliği. Belirtilen dizindeki öğeyi döndürür veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/extendedattributedefinitioncollection/item/
---
## ExtendedAttributeDefinitionCollection indexer

Belirtilen indeksteki öğeyi döndürür veya ayarlar.

```csharp
public ExtendedAttributeDefinition this[int index] { get; set; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Alınacak veya ayarlanacak öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

belirtilen indeksteki öğe.

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

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttributeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../extendedattributedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


