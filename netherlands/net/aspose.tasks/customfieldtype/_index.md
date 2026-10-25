---
title: "Enum CustomFieldType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CustomFieldType enum. Specificeert het type van een aangepast veld"
type: docs
weight: 380
url: /nl/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Specificeert het type van een aangepast veld.

```csharp
public enum CustomFieldType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Null | `0` | Geeft Null aangepast veldtype aan. |
| Cost | `1` | Geeft Kosten aangepast veldtype aan. |
| Date | `2` | Geeft Datum aangepast veldtype aan. |
| Duration | `3` | Geeft Duur aangepast veldtype aan. |
| Finish | `4` | Geeft Eind aangepast veldtype aan. |
| Flag | `5` | Geeft Vlag aangepast veldtype aan. |
| Number | `6` | Geeft Nummer aangepast veldtype aan. |
| Start | `7` | Geeft Start aangepast veldtype aan. |
| Text | `8` | Geeft Tekst aangepast veldtype aan. |
| OutlineCode | `9` | Geeft Outline Code aangepast veldtype aan. |
| RBS | `10` | Geeft RBS (Resource Breakdown Structure) aangepast veldtype aan. |

## Voorbeelden

Toont hoe je &lt;see cref="CustomFieldType" /&gt; (CustomFieldType.Text) gebruikt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// werken met definities...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


