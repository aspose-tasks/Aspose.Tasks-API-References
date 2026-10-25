---
title: "Enum CustomFieldType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.CustomFieldType enum. Spécifie le type d'un champ personnalisé"
type: docs
weight: 380
url: /fr/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Spécifie le type d’un champ personnalisé.

```csharp
public enum CustomFieldType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Null | `0` | Indique le type de champ personnalisé Null. |
| Cost | `1` | Indique le type de champ personnalisé Cost. |
| Date | `2` | Indique le type de champ personnalisé Date. |
| Duration | `3` | Indique le type de champ personnalisé Duration. |
| Finish | `4` | Indique le type de champ personnalisé Finish. |
| Flag | `5` | Indique le type de champ personnalisé Flag. |
| Number | `6` | Indique le type de champ personnalisé Number. |
| Start | `7` | Indique le type de champ personnalisé Start. |
| Text | `8` | Indique le type de champ personnalisé Text. |
| OutlineCode | `9` | Indique le type de champ personnalisé Outline Code. |
| RBS | `10` | Indique le type de champ personnalisé RBS (Resource Breakdown Structure). |

## Exemples

Montre comment utiliser &lt;see cref="CustomFieldType" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// travail avec les définitions...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


