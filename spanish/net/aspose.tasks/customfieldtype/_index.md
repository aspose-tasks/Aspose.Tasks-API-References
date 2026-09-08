---
title: "Enumeración CustomFieldType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.CustomFieldType. Especifica el tipo de un campo personalizado"
type: docs
weight: 380
url: /es/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Especifica el tipo de un campo personalizado.

```csharp
public enum CustomFieldType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Null | `0` | Indica el tipo de campo personalizado Nulo. |
| Cost | `1` | Indica el tipo de campo personalizado Costo. |
| Date | `2` | Indica el tipo de campo personalizado Fecha. |
| Duration | `3` | Indica el tipo de campo personalizado Duración. |
| Finish | `4` | Indica el tipo de campo personalizado Finalización. |
| Flag | `5` | Indica el tipo de campo personalizado Bandera. |
| Number | `6` | Indica el tipo de campo personalizado Número. |
| Start | `7` | Indica el tipo de campo personalizado Inicio. |
| Text | `8` | Indica el tipo de campo personalizado Texto. |
| OutlineCode | `9` | Indica el tipo de campo personalizado Código de esquema. |
| RBS | `10` | Indica el tipo de campo personalizado RBS (Estructura de Desglose de Recursos). |

## Ejemplos

Muestra cómo usar &lt;see cref="CustomFieldType" /&gt; (CustomFieldType.Text).

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// trabajar con definiciones...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


