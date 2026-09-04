---
title: "TimescaleFitBehavior"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un comportement utilisé pour aligner la zone de l'échelle de temps avec la largeur de la page."
type: docs
weight: 324
url: /fr/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Représente un comportement utilisé pour aligner la zone de l'échelle de temps avec la largeur de la page.
## Champs

| Champ | Description |
| --- | --- |
| [DefinedInView](#DefinedInView) | La section du calendrier est rendue selon la propriété View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage de la vue rendue. |
| [NoScaleToEndDate](#NoScaleToEndDate) | La section du calendrier est rendue exactement jusqu'à EndDate, même s'il y a un espace vide sur une page. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | La section du calendrier est rendue jusqu'à la fin (côté droit) de la dernière page. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Le moteur de rendu tentera d'aligner les dates afin que EndDate soit aligné avec la fin (côté droit) de la dernière page. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


La section du calendrier est rendue selon la propriété View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage de la vue rendue.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


La section du calendrier est rendue exactement jusqu'à EndDate, même s'il y a un espace vide sur une page.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


La section du calendrier est rendue jusqu'à la fin (côté droit) de la dernière page. Ainsi, la dernière date rendue peut dépasser EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Le moteur de rendu tentera d'aligner les dates afin que EndDate soit aligné avec la fin (côté droit) de la dernière page. Correspond à l'option "Page Setup \\ View \\ Fit timescale to end of page" de MS Project activée.

