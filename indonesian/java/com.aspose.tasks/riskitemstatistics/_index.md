---
title: "RiskItemStatistics"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili item yang menyimpan data statistik untuk tugas proyek yang dianalisis."
type: docs
weight: 265
url: /id/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Mewakili item yang menyimpan data statistik untuk tugas proyek yang dianalisis.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Mendapatkan nilai harapan dari item risiko. |
| [getItemType()](#getItemType--) | Mendapatkan sebuah instance dari enumerasi [RiskItemType](../../com.aspose.tasks/riskitemtype). |
| [getMaximum()](#getMaximum--) | Mendapatkan nilai maksimum yang dihasilkan selama simulasi Monte Carlo. |
| [getMinimum()](#getMinimum--) | Mendapatkan nilai minimum yang dihasilkan selama simulasi Monte Carlo. |
| [getPercentile(int percent)](#getPercentile-int-) | Mendapatkan nilai di bawah mana persentase tertentu dari sampel yang dihasilkan berada. |
| [getStandardDeviation()](#getStandardDeviation--) | Mendapatkan deviasi standar dari item risiko. |
| [toString()](#toString--) | Mengembalikan representasi string singkat dari sebuah item risiko. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Mendapatkan nilai harapan dari item risiko.

**Returns:**
java.util.Date - nilai yang diharapkan dari item risiko.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Mendapatkan sebuah instance dari enumerasi [RiskItemType](../../com.aspose.tasks/riskitemtype).

**Returns:**
int - sebuah instance dari enumerasi [RiskItemType](../../com.aspose.tasks/riskitemtype).
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Mendapatkan nilai maksimum yang dihasilkan selama simulasi Monte Carlo.

**Returns:**
java.util.Date - nilai maksimum yang dihasilkan selama simulasi Monte Carlo.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Mendapatkan nilai minimum yang dihasilkan selama simulasi Monte Carlo.

**Returns:**
java.util.Date - nilai minimum yang dihasilkan selama simulasi Monte Carlo.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Mendapatkan nilai di bawah mana persentase tertentu dari sampel yang dihasilkan berada.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| persen | int | persen yang ditentukan antara 0 dan 100. |

**Returns:**
java.util.Date - nilai di bawah mana persentase tertentu dari sampel yang dihasilkan berada.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Mendapatkan deviasi standar dari item risiko.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string pendek dari item risiko. Detail tepat dari representasi tidak ditentukan dan dapat berubah.

**Returns:**
java.lang.String - string pendek yang mewakili objek RiskItem.
