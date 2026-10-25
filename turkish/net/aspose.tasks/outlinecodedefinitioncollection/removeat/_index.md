---
title: "OutlineCodeDefinitionCollection.RemoveAt"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineCodeDefinitionCollection yöntemi. Belirtilen dizinde bir öğeyi kaldırır"
type: docs
weight: 120
url: /tr/net/aspose.tasks/outlinecodedefinitioncollection/removeat/
---
## OutlineCodeDefinitionCollection.RemoveAt method

Belirtilen dizindeki bir öğeyi kaldırır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Bir öğenin kaldırılacağı belirtilen sıfır tabanlı indeks. |

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

* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


