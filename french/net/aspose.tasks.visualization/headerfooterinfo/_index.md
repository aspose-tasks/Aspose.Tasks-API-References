---
title: "Classe HeaderFooterInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.HeaderFooterInfo. Représente le contenu visuel de l'en-tête/pied de page ou de la légende utilisé pour l'impression et le rendu des vues"
type: docs
weight: 3130
url: /fr/net/aspose.tasks.visualization/headerfooterinfo/
---
## HeaderFooterInfo class

Représente le contenu visuel de l'en-tête, du pied de page ou de la légende qui est utilisé pour l'impression \ le rendu des vues.

```csharp
public class HeaderFooterInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [HeaderFooterInfo](headerfooterinfo/)() | Initialise une nouvelle instance de la classe `HeaderFooterInfo`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CenteredImage](../../aspose.tasks.visualization/headerfooterinfo/centeredimage/) { get; set; } | Obtient ou définit l'image centrée à afficher dans l'élément parent. |
| [CenteredImageSize](../../aspose.tasks.visualization/headerfooterinfo/centeredimagesize/) { get; set; } | Obtient ou définit la taille affichée de l'image centrale. |
| [CenteredText](../../aspose.tasks.visualization/headerfooterinfo/centeredtext/) { get; set; } | Obtient ou définit le texte centré à afficher dans l'élément parent. |
| [LeftImage](../../aspose.tasks.visualization/headerfooterinfo/leftimage/) { get; set; } | Obtient ou définit l'image alignée à gauche à afficher dans l'élément parent. |
| [LeftImageSize](../../aspose.tasks.visualization/headerfooterinfo/leftimagesize/) { get; set; } | Obtient ou définit la taille affichée de l'image de gauche. |
| [LeftText](../../aspose.tasks.visualization/headerfooterinfo/lefttext/) { get; set; } | Obtient ou définit le texte aligné à gauche à afficher dans l'élément parent. |
| [RightImage](../../aspose.tasks.visualization/headerfooterinfo/rightimage/) { get; set; } | Obtient ou définit l'image alignée à droite à afficher dans l'élément parent. |
| [RightImageSize](../../aspose.tasks.visualization/headerfooterinfo/rightimagesize/) { get; set; } | Obtient ou définit la taille affichée de l'image de droite. |
| [RightText](../../aspose.tasks.visualization/headerfooterinfo/righttext/) { get; set; } | Obtient ou définit le texte aligné à droite à afficher dans l'élément parent. |

## Exemples

Affiche comment lire les informations d'en-tête/pied de page.

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

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


