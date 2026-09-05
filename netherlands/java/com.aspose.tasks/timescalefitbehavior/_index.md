---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een gedrag voor dat wordt gebruikt om het tijdschaalgebied uit te lijnen met de paginabreedte."
type: docs
weight: 324
url: /nl/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Stelt een gedrag voor dat wordt gebruikt om het tijdschaalgebied uit te lijnen met de paginabreedte.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [DefinedInView](#DefinedInView) | Kalendersectie wordt gerenderd volgens de View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage-eigenschap van de gerenderde View. |
| [NoScaleToEndDate](#NoScaleToEndDate) | Kalendersectie wordt exact tot EndDate gerenderd, zelfs als er een lege ruimte op een pagina is. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | Kalendersectie wordt gerenderd tot het einde (rechterkant) van de laatste pagina. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Renderengine zal proberen datums uit te lijnen zodat EndDate is uitgelijnd met het einde (rechterkant) van de laatste pagina. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Kalendersectie wordt gerenderd volgens de View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage-eigenschap van de gerenderde View.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


Kalendersectie wordt exact tot EndDate gerenderd, zelfs als er een lege ruimte op een pagina is.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


Kalendersectie wordt gerenderd tot het einde (rechterkant) van de laatste pagina. Daarom kan de laatst gerenderde datum EndDate overschrijden.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Renderengine zal proberen datums uit te lijnen zodat EndDate is uitgelijnd met het einde (rechterkant) van de laatste pagina. Komt overeen met de ingeschakelde optie "Page Setup \\ View \\ Fit timescale to end of page" van MS Project.

