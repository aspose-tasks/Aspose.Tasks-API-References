---
title: "Enumeración BackgroundPattern"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.BackgroundPattern. Especifica el patrón de fondo"
type: docs
weight: 100
url: /es/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Especifica el patrón de fondo.

```csharp
public enum BackgroundPattern
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Indica el patrón de fondo diagonal oscuro a la izquierda. |
| DarkDiagonalRight | `8` | Indica el patrón de fondo diagonal oscuro a la derecha. |
| DarkDither | `13` | Indica el patrón de fondo de tramado oscuro. |
| DarkFill | `4` | Indica el patrón de fondo de relleno oscuro. |
| DiagonalLeft | `5` | Indica el patrón de fondo diagonal izquierdo. |
| DiagonalRight | `6` | Indica el patrón de fondo diagonal derecho. |
| Hollow | `0` | Indica el patrón de fondo hueco. |
| LightDither | `11` | Indica el patrón de fondo de tramado claro. |
| LightFill | `2` | Indica el patrón de fondo de relleno claro. |
| MediumDither | `12` | Indica el patrón de fondo de tramado medio. |
| MediumFill | `3` | Indica el patrón de fondo de relleno medio. |
| MediumVerticalStripe | `10` | Indica el patrón de fondo de franjas verticales medianas. |
| SolidFill | `1` | Indica el patrón de fondo de relleno sólido. |
| ThinVerticalStripe | `9` | Indica el patrón de fondo de franjas verticales finas. |

## Ejemplos

Muestra cómo personalizar los estilos de texto que se utilizan para dar formato a diferentes elementos de texto en un proyecto.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


