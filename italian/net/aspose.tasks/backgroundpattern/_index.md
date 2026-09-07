---
title: "Enum BackgroundPattern"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.BackgroundPattern. Specifica il modello di sfondo"
type: docs
weight: 100
url: /it/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Specifica il modello di sfondo.

```csharp
public enum BackgroundPattern
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Indica il modello di sfondo diagonale sinistro scuro. |
| DarkDiagonalRight | `8` | Indica il modello di sfondo diagonale destro scuro. |
| DarkDither | `13` | Indica il modello di sfondo a reticolo scuro. |
| DarkFill | `4` | Indica il modello di sfondo di riempimento scuro. |
| DiagonalLeft | `5` | Indica il modello di sfondo diagonale sinistro. |
| DiagonalRight | `6` | Indica il modello di sfondo diagonale destro. |
| Hollow | `0` | Indica il modello di sfondo vuoto. |
| LightDither | `11` | Indica il modello di sfondo a retinatura leggera. |
| LightFill | `2` | Indica il modello di sfondo a riempimento leggero. |
| MediumDither | `12` | Indica il modello di sfondo a retinatura media. |
| MediumFill | `3` | Indica il modello di sfondo a riempimento medio. |
| MediumVerticalStripe | `10` | Indica il modello di sfondo a striscia verticale media. |
| SolidFill | `1` | Indica il modello di sfondo a riempimento solido. |
| ThinVerticalStripe | `9` | Indica il modello di sfondo a striscia verticale sottile. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


