---
title: "PrimaveraProjectProperties"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili properti khusus Primavera untuk sebuah proyek yang dibaca dari file Primavera XER atau P6XML."
type: docs
weight: 205
url: /id/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Mewakili properti khusus Primavera untuk proyek yang dibaca dari file Primavera (XER atau P6XML).
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Mengambil array proyek baseline dari proyek saat ini. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Mengambil metode untuk menentukan aktivitas kritis: pendekatan Jalur Terpanjang atau Total Float. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Mengambil nilai ambang yang digunakan untuk menentukan aktivitas kritis jika metode TotalFloat digunakan. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Mengambil Id dari proyek baseline saat ini. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Mengambil flag yang menentukan apakah mengabaikan hubungan aktivitas antar proyek. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Mengambil flag yang menentukan apakah aktivitas harus ditandai sebagai kritis saat menjadwalkan proyek. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Mengambil opsi yang menentukan kalender mana yang digunakan untuk menjadwalkan Lag Relasi dalam proyek Primavera. |
| [getShortName()](#getShortName--) | Mendapatkan nama pendek proyek (ID Proyek). |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Mengambil flag yang menentukan apakah tanggal selesai aktivitas harus dijadwalkan sebagai tanggal selesai yang diharapkan. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Mengambil array proyek baseline dari proyek saat ini. Berlaku untuk proyek yang dibaca dari file XML Primavera yang berisi baseline yang diekspor.

**Returns:**
com.aspose.tasks.Project[] - array proyek baseline dari proyek saat ini.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Mengambil metode untuk menentukan aktivitas kritis: pendekatan Jalur Terpanjang atau Total Float.

**Returns:**
int - metode untuk menentukan aktivitas kritis: pendekatan Jalur Terpanjang atau Total Float.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Mengambil nilai ambang yang digunakan untuk menentukan aktivitas kritis jika metode TotalFloat digunakan.

**Returns:**
java.lang.Double - nilai ambang yang digunakan untuk menentukan aktivitas kritis jika metode TotalFloat digunakan.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Mengambil Id dari proyek baseline saat ini. Berlaku untuk proyek yang dibaca dari file XML Primavera yang berisi baseline yang diekspor.

**Returns:**
int - Id dari proyek baseline saat ini.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Mengambil flag yang menentukan apakah mengabaikan hubungan aktivitas antar proyek.

**Returns:**
boolean - sebuah flag yang menentukan apakah mengabaikan hubungan aktivitas antara proyek.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Mengambil flag yang menentukan apakah aktivitas harus ditandai sebagai kritis saat menjadwalkan proyek.

**Returns:**
boolean - sebuah flag yang menentukan apakah aktivitas harus ditandai sebagai kritis saat menjadwalkan proyek.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Mengambil opsi yang menentukan kalender mana yang digunakan untuk menjadwalkan Lag Relasi dalam proyek Primavera.

**Returns:**
int - sebuah opsi yang menentukan kalender mana yang digunakan untuk menjadwalkan Relationship Lag dalam proyek Primavera.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Mendapatkan nama pendek proyek (ID Proyek).

**Returns:**
java.lang.String - nama pendek proyek (ID Proyek).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Mengambil flag yang menentukan apakah tanggal selesai aktivitas harus dijadwalkan sebagai tanggal selesai yang diharapkan.

**Returns:**
boolean - sebuah flag yang menentukan apakah tanggal selesai aktivitas harus dijadwalkan sebagai tanggal selesai yang diharapkan.
