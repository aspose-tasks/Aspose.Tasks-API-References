---
title: "Enum PrinterPaperSize"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.Visualization.PrinterPaperSize. Especifica el tamaño de papel que se utiliza para imprimir"
type: docs
weight: 3280
url: /es/net/aspose.tasks.visualization/printerpapersize/
---
## PrinterPaperSize enumeration

Especifica el tamaño de papel que se usa para imprimir.

```csharp
public enum PrinterPaperSize
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Custom | `1` | Indica que el tamaño de papel es definido por el usuario. |
| PaperLetter | `1` | Indica el tamaño de papel de impresora Envelope Letter (8.5 in. by 11 in.). |
| PaperLetterSmall | `2` | Indica el tamaño de papel de impresora Small Letter (8.5 in. by 11 in.). |
| PaperTabloid | `3` | Indica el tamaño de papel de impresora Tabloid (11 in. by 17 in.). |
| PaperLedger | `4` | Indica el tamaño de papel de impresora Ledger (17 in. by 11 in.). |
| PaperLegal | `5` | Indica el tamaño de papel de impresora Envelope legal (8.5 in. by 14 in.). |
| PaperStatement | `6` | Indica el tamaño de papel de impresora Statement (5.5 in. by 8.5 in.). |
| PaperExecutive | `7` | Indica el tamaño de papel de impresora Envelope executive (7.25 in. by 10.5 in.). |
| PaperA3 | `8` | Indica el tamaño de papel de impresora A3 (297 mm by 420 mm). |
| PaperA4 | `9` | Indica el tamaño de papel de impresora A4 (210 mm by 297 mm). |
| PaperA4Small | `10` | Indica el tamaño de papel de impresora Small A4 (210 mm by 297 mm). |
| PaperA5 | `11` | Indica el tamaño de papel de impresora A5 (148 mm by 210 mm). |
| PaperB4 | `12` | Indica el tamaño de papel de impresora B4 (250 mm by 353 mm). |
| PaperB5 | `13` | Indica el tamaño de papel de impresora B5 (176 mm by 250 mm). |
| PaperFolio | `14` | Indica el tamaño de papel de impresora Folio (8.5 in. by 13 in.). |
| PaperQuarto | `15` | Indica el tamaño de papel de impresora Quarto (215 mm by 275 mm). |
| PaperStandard10x14 | `16` | Indica el tamaño de papel de impresora Standard (10 in. by 14 in.). |
| PaperStandard11x17 | `17` | Indica el tamaño de papel de impresora Standard (11 in. by 17 in.). |
| PaperNote | `18` | Indica el tamaño de papel de impresora Note (8.5 in. by 11 in.). |
| PaperEnvelope10 | `20` | Indica el tamaño de papel de impresora Envelope10 (4.125 in. by 9.5 in.). |
| PaperCSheet | `24` | Indica el tamaño de papel de impresora C (17 in. by 22 in.). |
| PaperDSheet | `25` | Indica el tamaño de papel de impresora D (22 in. by 34 in.). |
| PaperESheet | `26` | Indica el tamaño de papel de impresora E (34 in. by 44 in.). |
| PaperEnvelopeMonarch | `37` | Indica el tamaño de papel de impresora Envelope Monarch (3.875 in. by 7.5 in.). |
| PaperStandard9x11 | `44` | Indica el tamaño de papel de impresora Standard (9 in. by 11 in.). |
| PaperStandard10x11 | `45` | Indica el tamaño de papel de impresora Standard (10 in. by 11 in.). |
| PaperStandard15x11 | `46` | Indica el tamaño estándar de papel para impresora (15 pulg. por 11 pulg.). |
| PaperA2 | `66` | Indica el tamaño de papel A2 para impresora (420 mm por 594 mm). |

## Ejemplos

Muestra cómo trabajar con la información de página de la vista de MS Project.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// permite modificar la vista predeterminada
var info = project.DefaultView.PageInfo;

Console.WriteLine("Modify Page Info: " + info.Name);

// permite modificar los márgenes
info.Margins.Left = 10d;
info.Margins.Top = 10d;
info.Margins.Right = 10d;
info.Margins.Bottom = 10d;

// modifiquemos la configuración de página
info.PageSettings.IsPortrait = true;
info.PageSettings.PaperSize = PrinterPaperSize.PaperA4;

// modifiquemos la configuración de vista de página
// establece un valor que indica si se imprimen notas.
info.PageViewSettings.PrintNotes = true;

var header = new HeaderFooterInfo
{
    LeftText = "Left header text",
    CenteredText = "Centered header text",
    RightText = "Right header text"
};
var legend = new PageLegend
{
    LeftText =  "Left legend text",
    CenteredText = "Centered legend text",
    RightText = "Right legend text"
};
var footer = new HeaderFooterInfo
{
    LeftText = "Left footer text",
    CenteredText = "Centered footer text",
    RightText = "Right footer text"
};

info.Header = header;
info.Legend = legend;
info.Footer = footer;

// trabajar con el proyecto...
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


