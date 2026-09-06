---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Zaman ölçeği alanını sayfa genişliğiyle hizalamak için kullanılan bir davranışı temsil eder."
type: docs
weight: 324
url: /tr/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Zaman ölçeği alanını sayfa genişliğiyle hizalamak için kullanılan bir davranışı temsil eder.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [DefinedInView](#DefinedInView) | Takvim bölümü, render edilen Görünüm'ün View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage özelliğine göre işlenir. |
| [NoScaleToEndDate](#NoScaleToEndDate) | Takvim bölümü, bir sayfada boş alan olsa bile EndDate'e tam olarak işlenir. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | Takvim bölümü, son sayfanın sonuna (sağ tarafına) işlenir. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Render motoru, tarihleri EndDate'in son sayfanın sonuna (sağ tarafına) hizalanacak şekilde ayarlamaya çalışır. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Takvim bölümü, render edilen Görünüm'ün View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage özelliğine göre işlenir.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


Takvim bölümü, bir sayfada boş alan olsa bile EndDate'e tam olarak işlenir.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


Takvim bölümü, son sayfanın sonuna (sağ tarafına) işlenir. Bu nedenle son işlenen tarih EndDate'i aşabilir.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Render motoru, tarihleri EndDate'in son sayfanın sonuna (sağ tarafına) hizalanacak şekilde ayarlamaya çalışır. MS Project'in \"Page Setup \\\\ View \\\\ Fit timescale to end of page\" seçeneği etkinleştirildiğinde karşılık gelir.

