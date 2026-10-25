---
title: "TextStyle.ItemType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TextStyle. Obtiene o establece TextItemType del estilo de texto"
type: docs
weight: 60
url: /es/net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

Obtiene o establece [`TextItemType`](../../textitemtype/) del estilo de texto.

```csharp
public virtual TextItemType ItemType { get; set; }
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

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


