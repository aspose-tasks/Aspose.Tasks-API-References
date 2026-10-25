---
title: "Classe TextStyle"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.TextStyle classe. Cambia lo stile visivo del testo per un elemento nella visualizzazione del progetto"
type: docs
weight: 3420
url: /it/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Modifica lo stile visivo del testo per un elemento nella visualizzazione del progetto.

```csharp
public class TextStyle
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Inizializza una nuova istanza della classe `TextStyle` con le impostazioni predefinite. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Inizializza una nuova istanza della classe `TextStyle` con le impostazioni del carattere specificate. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Inizializza una nuova istanza della classe `TextStyle` con il carattere predefinito e lo stile del carattere specificato. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Inizializza una nuova istanza della classe `TextStyle` con il carattere predefinito e la dimensione e lo stile del carattere specificati. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo dello stile del testo. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Ottiene o imposta il motivo di sfondo dello stile del testo. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Ottiene o imposta il colore del testo. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Ottiene o imposta il carattere dello stile del testo. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Ottiene o imposta il [`TextItemType`](../textitemtype/) dello stile del testo. |

## Esempi

Mostra come personalizzare gli stili di testo che vengono usati per formattare diversi elementi di testo in un progetto.

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

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


