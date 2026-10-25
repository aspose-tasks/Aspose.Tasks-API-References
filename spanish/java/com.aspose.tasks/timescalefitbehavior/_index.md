---
title: "TimescaleFitBehavior"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa un comportamiento utilizado para alinear el área de escala de tiempo con el ancho de página."
type: docs
weight: 324
url: /es/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Representa un comportamiento utilizado para alinear el área de escala de tiempo con el ancho de página.
## Campos

| Campo | Descripción |
| --- | --- |
| [DefinedInView](#DefinedInView) | La sección del calendario se renderiza de acuerdo con la propiedad View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage de la vista renderizada. |
| [NoScaleToEndDate](#NoScaleToEndDate) | La sección del calendario se renderiza exactamente hasta EndDate, incluso si hay un espacio vacío en una página. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | La sección del calendario se renderiza hasta el final (lado derecho) de la última página. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | El motor de renderizado intentará alinear las fechas de modo que EndDate quede alineado con el final (lado derecho) de la última página. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


La sección del calendario se renderiza de acuerdo con la propiedad View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage de la vista renderizada.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


La sección del calendario se renderiza exactamente hasta EndDate, incluso si hay un espacio vacío en una página.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


La sección del calendario se renderiza hasta el final (lado derecho) de la última página. Por lo tanto, la última fecha renderizada puede exceder EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


El motor de renderizado intentará alinear las fechas de modo que EndDate quede alineado con el final (lado derecho) de la última página. Corresponde a la opción "Page Setup \\ View \\ Fit timescale to end of page" de MS Project habilitada.

