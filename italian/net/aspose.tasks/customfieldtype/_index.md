---
title: "Enum CustomFieldType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.CustomFieldType enum. Specifica il tipo di un campo personalizzato"
type: docs
weight: 380
url: /it/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Specifica il tipo di campo personalizzato.

```csharp
public enum CustomFieldType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Null | `0` | Indica il tipo di campo personalizzato Null. |
| Cost | `1` | Indica il tipo di campo personalizzato Cost. |
| Date | `2` | Indica il tipo di campo personalizzato Date. |
| Duration | `3` | Indica il tipo di campo personalizzato Duration. |
| Finish | `4` | Indica il tipo di campo personalizzato Finish. |
| Flag | `5` | Indica il tipo di campo personalizzato Flag. |
| Number | `6` | Indica il tipo di campo personalizzato Number. |
| Start | `7` | Indica il tipo di campo personalizzato Start. |
| Text | `8` | Indica il tipo di campo personalizzato Text. |
| OutlineCode | `9` | Indica il tipo di campo personalizzato Outline Code. |
| RBS | `10` | Indica il tipo di campo personalizzato RBS (Resource Breakdown Structure). |

## Esempi

Mostra come utilizzare &lt;see cref="CustomFieldType" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// lavorare con le definizioni...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


