---
title: "TextStyle.BackgroundColor"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TextStyle. Obtiene o establece el color de fondo del estilo de texto. Color"
type: docs
weight: 20
url: /es/net/aspose.tasks.visualization/textstyle/backgroundcolor/
---
## TextStyle.BackgroundColor property

Obtiene o establece el color de fondo del estilo de texto. [`Color`](../color/).

```csharp
public Color BackgroundColor { get; set; }
```

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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


