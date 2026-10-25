---
title: "TextStyle.TextStyle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor TextStyle. Inicializa una nueva instancia de la clase TextStyle con la configuración predeterminada"
type: docs
weight: 10
url: /es/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Inicializa una nueva instancia de la clase [`TextStyle`](../) con la configuración predeterminada.

```csharp
public TextStyle()
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

---

## TextStyle(float, FontStyles) {#constructor_3}

Inicializa una nueva instancia de la clase [`TextStyle`](../) con la fuente predeterminada y el tamaño y estilo de fuente especificados.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontSize | Single | Tamaño de fuente de TextStyle. |
| fontStyle | FontStyles | Estilo de fuente de TextStyle. |

### Ver también

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Inicializa una nueva instancia de la clase [`TextStyle`](../) con la fuente predeterminada y el estilo de fuente especificado.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontStyle | FontStyles | Estilo de fuente a aplicar a la fuente predeterminada. |

### Ver también

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Inicializa una nueva instancia de la clase [`TextStyle`](../) con la configuración de fuente especificada.

```csharp
public TextStyle(FontDescriptor font)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| font | FontDescriptor | Fuente de TextStyle. |

### Ver también

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


