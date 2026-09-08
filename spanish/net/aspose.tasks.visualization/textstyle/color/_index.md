---
title: "TextStyle.Color"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TextStyle. Obtiene o establece el color del texto"
type: docs
weight: 40
url: /es/net/aspose.tasks.visualization/textstyle/color/
---
## TextStyle.Color property

Obtiene o establece el color del texto.

```csharp
public Color Color { get; set; }
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


