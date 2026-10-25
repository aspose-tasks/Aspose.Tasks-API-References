---
title: "PrimaveraTaskProperties"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili properti khusus Primavera untuk sebuah tugas yang dibaca dari file Primavera XER atau P6XML."
type: docs
weight: 209
url: /id/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Mewakili properti khusus Primavera untuk tugas yang dibaca dari file Primavera (XER atau P6XML).
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getActivityId()](#getActivityId--) | Mendapatkan bidang id aktivitas - pengidentifikasi unik tugas yang digunakan oleh Primavera. |
| [getActivityType()](#getActivityType--) | Mendapatkan nilai bidang 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Mendapatkan nilai biaya pengeluaran aktual. |
| [getActualLaborCost()](#getActualLaborCost--) | Mendapatkan nilai biaya tenaga kerja aktual . |
| [getActualLaborUnits()](#getActualLaborUnits--) | Mendapatkan nilai satuan tenaga kerja aktual. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Mendapatkan nilai biaya material aktual. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Mendapatkan nilai satuan non tenaga kerja aktual. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Mendapatkan nilai biaya non tenaga kerja aktual . |
| [getActualTotalCost()](#getActualTotalCost--) | Mendapatkan total nilai biaya aktual. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Mendapatkan nilai biaya pengeluaran yang dianggarkan (atau direncanakan). |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Mendapatkan nilai biaya tenaga kerja yang dianggarkan (atau direncanakan) . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Mendapatkan nilai biaya material yang dianggarkan (atau direncanakan). |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Mendapatkan nilai biaya non tenaga kerja yang dianggarkan (atau direncanakan) . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Mendapatkan total nilai biaya yang dianggarkan (atau direncanakan). |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Mendapatkan nilai persentase penyelesaian durasi. |
| [getDurationType()](#getDurationType--) | Mendapatkan nilai bidang 'Duration Type' dari aktivitas. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Mendapatkan nilai bidang '% Complete Type' dari aktivitas. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Mendapatkan nilai Persentase Fisik yang Selesai. |
| [getPlannedDuration()](#getPlannedDuration--) | Mendapatkan durasi asli atau yang direncanakan -- total waktu kerja dari tanggal mulai yang direncanakan tugas hingga tanggal selesai yang direncanakan.. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Mendapatkan tanggal kendala utama. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Mendapatkan tipe kendala utama. |
| [getRawActivityType()](#getRawActivityType--) | Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang 'Activity Type' aktivitas. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang '% Complete Type' aktivitas. |
| [getRawDurationType()](#getRawDurationType--) | Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang 'Duration Type' aktivitas. |
| [getRawStatus()](#getRawStatus--) | Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang 'Status' aktivitas. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Mendapatkan tanggal selesai awal yang tersisa - tanggal ketika pekerjaan yang tersisa untuk aktivitas dijadwalkan selesai. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Mendapatkan tanggal mulai awal yang tersisa - tanggal ketika pekerjaan yang tersisa untuk aktivitas dijadwalkan dimulai. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Mendapatkan nilai biaya pengeluaran yang tersisa. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Mendapatkan nilai satuan tenaga kerja yang tersisa. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Mendapatkan tanggal selesai akhir terlambat yang tersisa. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Mendapatkan tanggal mulai awal terlambat yang tersisa. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Mendapatkan nilai satuan non tenaga kerja yang tersisa. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Mendapatkan tanggal batasan sekunder. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Mendapatkan tipe batasan sekunder. |
| [getSequenceNumber()](#getSequenceNumber--) | Mendapatkan nomor urut item WBS (tugas rangkuman). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Mendapatkan nilai persentase penyelesaian satuan. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Mendapatkan bidang id aktivitas - pengidentifikasi unik tugas yang digunakan oleh Primavera.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
java.lang.String - sebuah bidang id aktivitas - pengidentifikasi unik tugas yang digunakan oleh Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Mendapatkan nilai bidang 'Activity Type'.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
int - nilai bidang 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Mendapatkan nilai biaya pengeluaran aktual.

**Returns:**
java.math.BigDecimal - nilai biaya pengeluaran aktual.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Mendapatkan nilai biaya tenaga kerja aktual .

**Returns:**
java.math.BigDecimal - nilai biaya tenaga kerja aktual.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Mendapatkan nilai satuan tenaga kerja aktual.

**Returns:**
double - nilai satuan tenaga kerja aktual.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Mendapatkan nilai biaya material aktual.

**Returns:**
java.math.BigDecimal - nilai biaya material aktual.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Mendapatkan nilai satuan non tenaga kerja aktual.

**Returns:**
double - nilai satuan non tenaga kerja aktual.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Mendapatkan nilai biaya non tenaga kerja aktual .

**Returns:**
java.math.BigDecimal - nilai biaya non tenaga kerja aktual.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Mendapatkan total nilai biaya aktual.

**Returns:**
java.math.BigDecimal - total nilai biaya aktual.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Mendapatkan nilai biaya pengeluaran yang dianggarkan (atau direncanakan).

**Returns:**
java.math.BigDecimal - nilai biaya pengeluaran yang dianggarkan (atau direncanakan).
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Mendapatkan nilai biaya tenaga kerja yang dianggarkan (atau direncanakan) .

**Returns:**
java.math.BigDecimal - nilai biaya tenaga kerja yang dianggarkan (atau direncanakan).
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Mendapatkan nilai biaya material yang dianggarkan (atau direncanakan).

**Returns:**
java.math.BigDecimal - nilai biaya material yang dianggarkan (atau direncanakan).
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Mendapatkan nilai biaya non tenaga kerja yang dianggarkan (atau direncanakan) .

**Returns:**
java.math.BigDecimal - nilai biaya non tenaga kerja yang dianggarkan (atau direncanakan).
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Mendapatkan total nilai biaya yang dianggarkan (atau direncanakan).

**Returns:**
java.math.BigDecimal - total nilai biaya yang dianggarkan (atau direncanakan).
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Mendapatkan nilai persentase penyelesaian durasi.

**Returns:**
double - nilai persentase penyelesaian durasi.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Mendapatkan nilai bidang 'Duration Type' dari aktivitas.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
int - nilai bidang 'Duration Type' dari aktivitas.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Mendapatkan nilai bidang '% Complete Type' dari aktivitas.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
int - nilai dari bidang '% Complete Type' pada aktivitas.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Mendapatkan nilai Persentase Fisik yang Selesai.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
double - nilai dari Physical Percent Complete.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Mendapatkan durasi asli atau yang direncanakan -- total waktu kerja dari tanggal mulai yang direncanakan tugas hingga tanggal selesai yang direncanakan..

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Mendapatkan tanggal kendala utama.

**Returns:**
java.util.Date - tanggal dari primary constraint.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Mendapatkan tipe kendala utama.

**Returns:**
int - tipe dari primary constraint.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang 'Activity Type' aktivitas.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
java.lang.String - representasi teks mentah (seperti dalam file sumber) dari bidang 'Activity Type' pada aktivitas.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang '% Complete Type' aktivitas.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
java.lang.String - representasi teks mentah (seperti dalam file sumber) dari bidang '% Complete Type' pada aktivitas.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang 'Duration Type' aktivitas.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
java.lang.String - representasi teks mentah (seperti dalam file sumber) dari bidang 'Duration Type' pada aktivitas.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Mendapatkan representasi teks mentah (seperti dalam file sumber) dari bidang 'Status' aktivitas.

--------------------

Hanya berlaku untuk aktivitas (tugas non-rangkuman).

**Returns:**
java.lang.String - representasi teks mentah (seperti dalam file sumber) dari bidang 'Status' pada aktivitas.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Mendapatkan tanggal selesai awal yang tersisa - tanggal ketika pekerjaan yang tersisa untuk aktivitas dijadwalkan selesai.

**Returns:**
java.util.Date - tanggal selesai awal yang tersisa - tanggal ketika pekerjaan yang tersisa untuk aktivitas dijadwalkan selesai.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Mendapatkan tanggal mulai awal yang tersisa - tanggal ketika pekerjaan yang tersisa untuk aktivitas dijadwalkan dimulai.

**Returns:**
java.util.Date - tanggal mulai awal yang tersisa - tanggal ketika pekerjaan yang tersisa untuk aktivitas dijadwalkan dimulai.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Mendapatkan nilai biaya pengeluaran yang tersisa.

**Returns:**
java.math.BigDecimal - nilai dari biaya pengeluaran yang tersisa.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Mendapatkan nilai satuan tenaga kerja yang tersisa.

**Returns:**
double - nilai dari unit tenaga kerja yang tersisa.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Mendapatkan tanggal selesai akhir terlambat yang tersisa.

**Returns:**
java.util.Date - tanggal selesai akhir yang tersisa.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Mendapatkan tanggal mulai awal terlambat yang tersisa.

**Returns:**
java.util.Date - tanggal mulai akhir yang tersisa.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Mendapatkan nilai satuan non tenaga kerja yang tersisa.

**Returns:**
double - nilai dari unit non tenaga kerja yang tersisa.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Mendapatkan tanggal batasan sekunder.

**Returns:**
java.util.Date - tanggal dari secondary constraint.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Mendapatkan tipe batasan sekunder.

**Returns:**
int - tipe dari secondary constraint.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Mendapatkan nomor urut dari item WBS (tugas rangkuman). Ini digunakan untuk mengurutkan tugas rangkuman di Primavera.

--------------------

Berlaku untuk item WBS (tugas rangkuman).

**Returns:**
int - nomor urut dari item WBS (tugas rangkuman).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Mendapatkan nilai persentase penyelesaian satuan.

**Returns:**
double - nilai dari persentase penyelesaian unit.
