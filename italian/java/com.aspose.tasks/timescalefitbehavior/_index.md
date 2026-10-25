---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un comportamento usato per allineare l'area della scala temporale alla larghezza della pagina."
type: docs
weight: 324
url: /it/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Rappresenta un comportamento usato per allineare l'area della scala temporale alla larghezza della pagina.
## Campi

| Campo | Descrizione |
| --- | --- |
| [DefinedInView](#DefinedInView) | La sezione del calendario è resa in base alla proprietà View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage della Vista resa. |
| [NoScaleToEndDate](#NoScaleToEndDate) | La sezione del calendario è resa esattamente fino a EndDate, anche se c'è uno spazio vuoto su una pagina. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | La sezione del calendario è resa fino alla fine (lato destro) dell'ultima pagina. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Il motore di rendering cercherà di allineare le date in modo che EndDate sia allineato con la fine (lato destro) dell'ultima pagina. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


La sezione del calendario è resa in base alla proprietà View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage della Vista resa.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


La sezione del calendario è resa esattamente fino a EndDate, anche se c'è uno spazio vuoto su una pagina.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


La sezione del calendario è resa fino alla fine (lato destro) dell'ultima pagina. Pertanto l'ultima data resa potrebbe superare EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Il motore di rendering cercherà di allineare le date in modo che EndDate sia allineato con la fine (lato destro) dell'ultima pagina. Corrisponde all'opzione "Impostazione pagina \\ Visualizza \\ Adatta la scala temporale alla fine della pagina" di MS Project attivata.

