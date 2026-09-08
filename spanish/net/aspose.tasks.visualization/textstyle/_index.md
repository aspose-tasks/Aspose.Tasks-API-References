---
title: "Clase TextStyle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.TextStyle clase. Cambia el estilo visual del texto para un elemento en la vista del proyecto"
type: docs
weight: 3420
url: /es/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Cambiar el estilo visual del texto para un elemento en la vista del proyecto.

```csharp
public class TextStyle
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Inicializa una nueva instancia de la clase `TextStyle` con la configuración predeterminada. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Inicializa una nueva instancia de la clase `TextStyle` con los ajustes de fuente especificados. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Inicializa una nueva instancia de la clase `TextStyle` con la fuente predeterminada y el estilo de fuente especificado. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Inicializa una nueva instancia de la clase `TextStyle` con la fuente predeterminada y el tamaño y estilo de fuente especificados. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Obtiene o establece el color de fondo del estilo de texto. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Obtiene o establece el patrón de fondo del estilo de texto. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Obtiene o establece el color del texto. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Obtiene o establece la fuente del estilo de texto. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Obtiene o establece [`TextItemType`](../textitemtype/) del estilo de texto. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


