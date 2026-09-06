---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett beteende som används för att justera tidslinjeområdet med sidbredden."
type: docs
weight: 324
url: /sv/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Representerar ett beteende som används för att justera tidslinjeområdet med sidbredden.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [DefinedInView](#DefinedInView) | Kalendersektionen renderas enligt egenskapen View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage för den renderade vyn. |
| [NoScaleToEndDate](#NoScaleToEndDate) | Kalendersektionen renderas exakt till EndDate, även om det finns ett tomt utrymme på en sida. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | Kalendersektionen renderas till slutet (höger sida) av den sista sidan. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Renderingsmotorn kommer att försöka justera datum så att EndDate är justerat med slutet (höger sida) av den sista sidan. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Kalendersektionen renderas enligt egenskapen View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage för den renderade vyn.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


Kalendersektionen renderas exakt till EndDate, även om det finns ett tomt utrymme på en sida.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


Kalendersektionen renderas till slutet (höger sida) av den sista sidan. Därmed kan det sista renderade datumet överstiga EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Renderingsmotorn kommer att försöka justera datum så att EndDate är justerat med slutet (höger sida) av den sista sidan. Detta motsvarar att alternativet \"Page Setup \\\\ View \\\\ Fit timescale to end of page\" i MS Project är aktiverat.

