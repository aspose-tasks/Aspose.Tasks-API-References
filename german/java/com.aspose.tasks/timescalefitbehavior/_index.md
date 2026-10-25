---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt ein Verhalten dar, das verwendet wird, um den Zeitskala-Bereich an die Seitenbreite anzupassen."
type: docs
weight: 324
url: /de/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Stellt ein Verhalten dar, das verwendet wird, um den Zeitskala-Bereich an die Seitenbreite anzupassen.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [DefinedInView](#DefinedInView) | Kalenderabschnitt wird gemäß der Eigenschaft View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage der gerenderten Ansicht dargestellt. |
| [NoScaleToEndDate](#NoScaleToEndDate) | Kalenderabschnitt wird exakt bis zum EndDate dargestellt, selbst wenn auf einer Seite ein leerer Raum verbleibt. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | Kalenderabschnitt wird bis zum Ende (rechte Seite) der letzten Seite dargestellt. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Die Rendering‑Engine versucht, die Daten so auszurichten, dass EndDate mit dem Ende (rechte Seite) der letzten Seite übereinstimmt. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Kalenderabschnitt wird gemäß der Eigenschaft View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage der gerenderten Ansicht dargestellt.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


Kalenderabschnitt wird exakt bis zum EndDate dargestellt, selbst wenn auf einer Seite ein leerer Raum verbleibt.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


Kalenderabschnitt wird bis zum Ende (rechte Seite) der letzten Seite dargestellt. Daher kann das zuletzt gerenderte Datum das EndDate überschreiten.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Die Rendering-Engine versucht, Daten so auszurichten, dass EndDate am Ende (rechte Seite) der letzten Seite ausgerichtet ist. Entspricht der aktivierten Option "Page Setup \\ View \\ Fit timescale to end of page" von MS Project.

