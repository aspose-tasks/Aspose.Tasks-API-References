---
title: "SaveOptions.TextStyles"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto"
type: docs
weight: 190
url: /es/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Obtiene o establece la lista de estilos de texto que se aplican durante la renderización de una vista de proyecto.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Observaciones

Estos estilos sobrescriben los estilos definidos en GanttCharView.TextStyles.

## Ejemplos

Muestra cómo usar los estilos de texto de las opciones de guardado que se utilizan para dar formato a diferentes elementos de texto en un proyecto.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Ver también

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


