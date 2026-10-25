---
title: "TimescaleFitBehavior"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili perilaku yang digunakan untuk menyelaraskan area skala waktu dengan lebar halaman."
type: docs
weight: 324
url: /id/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Mewakili perilaku yang digunakan untuk menyelaraskan area skala waktu dengan lebar halaman.
## Bidang

| Bidang | Deskripsi |
| --- | --- |
| [DefinedInView](#DefinedInView) | Bagian kalender dirender sesuai properti View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage dari Tampilan yang dirender. |
| [NoScaleToEndDate](#NoScaleToEndDate) | Bagian kalender dirender tepat hingga EndDate, bahkan jika ada ruang kosong pada halaman. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | Bagian kalender dirender hingga akhir (sisi kanan) halaman terakhir. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Mesin rendering akan mencoba menyelaraskan tanggal sehingga EndDate sejajar dengan akhir (sisi kanan) halaman terakhir. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Bagian kalender dirender sesuai properti View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage dari Tampilan yang dirender.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


Bagian kalender dirender tepat hingga EndDate, bahkan jika ada ruang kosong pada halaman.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


Bagian kalender dirender hingga akhir (sisi kanan) halaman terakhir. Oleh karena itu tanggal yang dirender terakhir mungkin melebihi EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Mesin rendering akan mencoba menyelaraskan tanggal sehingga EndDate sejajar dengan akhir (sisi kanan) halaman terakhir. Sesuai dengan opsi "Page Setup \\ View \\ Fit timescale to end of page" pada MS Project yang diaktifkan.

