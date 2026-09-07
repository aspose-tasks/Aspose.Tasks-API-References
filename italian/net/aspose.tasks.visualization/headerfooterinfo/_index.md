---
title: "Classe HeaderFooterInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.HeaderFooterInfo. Rappresenta il contenuto visivo dell'intestazione, piè di pagina o legenda utilizzato per la stampa e il rendering delle visualizzazioni"
type: docs
weight: 3130
url: /it/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Rappresenta il contenuto visivo dell'intestazione, del piè di pagina o della legenda utilizzato per la stampa \ rendering delle visualizzazioni.

```csharp
public class HeaderFooterInfo
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Inizializza una nuova istanza della classe `HeaderFooterInfo`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Ottiene o imposta l'immagine centrata da visualizzare nell'elemento genitore. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Ottiene o imposta la dimensione visualizzata dell'immagine centrale. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Ottiene o imposta il testo centrato da visualizzare nell'elemento genitore. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Ottiene o imposta l'immagine allineata a sinistra da visualizzare nell'elemento padre. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Ottiene o imposta la dimensione visualizzata dell'immagine a sinistra. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Ottiene o imposta il testo allineato a sinistra da visualizzare nell'elemento padre. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Ottiene o imposta l'immagine allineata a destra da visualizzare nell'elemento padre. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Ottiene o imposta la dimensione visualizzata dell'immagine a destra. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Ottiene o imposta il testo allineato a destra da visualizzare nell'elemento padre. |

## Esempi

Mostra come leggere le informazioni dell'intestazione/piè di pagina.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");
var info = project.DefaultView.PageInfo;

Console.WriteLine("Header left text: {0} ", info.Header.LeftText);
Console.WriteLine("Header left image: {0} ", info.Header.LeftImage);
Console.WriteLine("Header left image size: {0} ", info.Header.LeftImageSize);
Console.WriteLine("Header center text: {0} ", info.Header.CenteredText);
Console.WriteLine("Header center image: {0} ", info.Header.CenteredImage);
Console.WriteLine("Header center image size: {0} ", info.Header.CenteredImageSize);
Console.WriteLine("Header right text: {0} ", info.Header.RightText);
Console.WriteLine("Header right image: {0} ", info.Header.RightImage);
Console.WriteLine("Header right image size: {0} ", info.Header.RightImageSize);
Console.WriteLine();
Console.WriteLine("Footer left text: {0} ", info.Footer.LeftText);
Console.WriteLine("Footer left image: {0} ", info.Footer.LeftImage);
Console.WriteLine("Footer left image size: {0} ", info.Footer.LeftImageSize);
Console.WriteLine("Footer center text: {0} ", info.Footer.CenteredText);
Console.WriteLine("Footer center image: {0} ", info.Footer.CenteredImage);
Console.WriteLine("Footer center size: {0} ", info.Footer.CenteredImageSize);
Console.WriteLine("Footer right text: {0} ", info.Footer.RightText);
Console.WriteLine("Footer right image: {0} ", info.Footer.RightImage);
Console.WriteLine("Footer right image size: {0} ", info.Footer.RightImageSize);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


