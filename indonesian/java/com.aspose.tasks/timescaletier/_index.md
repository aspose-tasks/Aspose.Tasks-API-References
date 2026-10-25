---
title: "TimescaleTier"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili satu tingkat skala waktu pada Gantt Chart."
type: docs
weight: 325
url: /id/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Mewakili satu tingkat skala waktu pada Gantt Chart.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Menginisialisasi instance baru dari kelas [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Menginisialisasi instance baru dari kelas [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getAlignment()](#getAlignment--) | Mendapatkan cara menyelaraskan label dalam setiap periode waktu tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Mendapatkan interval satuan waktu di mana label ditampilkan untuk tier. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Mendapatkan fungsi callback untuk menangani rendering tick tanggal di tier ini. |
| [getLabel()](#getLabel--) | Mendapatkan label tanggal [DateLabel](../../com.aspose.tasks/datelabel) untuk tier skala waktu. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Mendapatkan flag yang menentukan apakah label tanggal harus dirender pada setiap halaman ketika periode waktu melintasi beberapa halaman. |
| [getShowTicks()](#getShowTicks--) | Mendapatkan nilai yang menunjukkan apakah menampilkan tanda tick yang memisahkan periode waktu dalam tier. |
| [getUnit()](#getUnit--) | Mendapatkan satuan skala waktu [TimescaleUnit](../../com.aspose.tasks/timescaleunit) untuk tier skala waktu. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Mendapatkan nilai yang menunjukkan apakah label tier didasarkan pada tahun fiskal. |
| [setAlignment(int value)](#setAlignment-int-) | Mengatur cara menyelaraskan label dalam setiap periode waktu tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Mengatur interval satuan waktu di mana label ditampilkan untuk tier. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Mengatur fungsi callback untuk menangani rendering tick tanggal di tier ini. |
| [setLabel(int value)](#setLabel-int-) | Mengatur label tanggal [DateLabel](../../com.aspose.tasks/datelabel) untuk tier skala waktu. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Mengatur flag yang menentukan apakah label tanggal harus dirender pada setiap halaman ketika periode waktu melintasi beberapa halaman. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Mengatur nilai yang menunjukkan apakah menampilkan tanda tick yang memisahkan periode waktu dalam tier. |
| [setUnit(int value)](#setUnit-int-) | Mengatur satuan skala waktu [TimescaleUnit](../../com.aspose.tasks/timescaleunit) untuk tier skala waktu. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Mengatur nilai yang menunjukkan apakah label tier didasarkan pada tahun fiskal. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Menginisialisasi instance baru dari kelas [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Menginisialisasi instance baru dari kelas [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| unit | int | Satuan skala waktu [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | Jumlah satuan [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Mendapatkan cara menyelaraskan label dalam setiap periode waktu tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - cara menyelaraskan label dalam setiap periode waktu tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Mendapatkan interval satuan waktu di mana label ditampilkan untuk tier. Nilai default adalah 1.

**Returns:**
int - interval satuan waktu di mana label ditampilkan untuk tier.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Mendapatkan fungsi callback untuk menangani rendering tick tanggal di tier ini.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Mendapatkan label tanggal [DateLabel](../../com.aspose.tasks/datelabel) untuk tier skala waktu.

**Returns:**
int - label tanggal [DateLabel](../../com.aspose.tasks/datelabel) untuk tier skala waktu.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Mendapatkan flag yang menentukan apakah label tanggal harus dirender pada setiap halaman ketika periode waktu melintasi beberapa halaman. Jika nilai 'true', ketika periode waktu melintasi beberapa halaman, label tanggal untuk periode tersebut dirender pada setiap halaman. Jika nilai 'false', label tanggal hanya dirender sekali sesuai nilai properti `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)).

--------------------

Tidak memiliki padanan di MS Project.

**Returns:**
boolean - flag yang menentukan apakah label tanggal harus dirender pada setiap halaman ketika periode waktu meluas ke beberapa halaman.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Mendapatkan nilai yang menunjukkan apakah menampilkan tanda tick yang memisahkan periode waktu dalam tier.

**Returns:**
boolean - nilai yang menunjukkan apakah menampilkan tanda centang yang memisahkan periode waktu dalam tier.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Mendapatkan unit skala waktu [TimescaleUnit](../../com.aspose.tasks/timescaleunit) untuk tier skala waktu. Nilai default adalah [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - unit skala waktu [TimescaleUnit](../../com.aspose.tasks/timescaleunit) untuk tier skala waktu.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Mendapatkan nilai yang menunjukkan apakah label tier didasarkan pada tahun fiskal.

**Returns:**
boolean - nilai yang menunjukkan apakah label tier didasarkan pada tahun fiskal.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Mengatur cara menyelaraskan label dalam setiap periode waktu tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | cara menyelaraskan label dalam setiap periode waktu tier ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Mengatur interval satuan waktu di mana label ditampilkan untuk tier. Nilai default adalah 1.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | interval satuan waktu di mana label ditampilkan untuk tier. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Mengatur fungsi callback untuk menangani rendering tick tanggal di tier ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | fungsi callback untuk menangani perenderan tanda tanggal dalam tier ini. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Mengatur label tanggal [DateLabel](../../com.aspose.tasks/datelabel) untuk tier skala waktu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | label tanggal [DateLabel](../../com.aspose.tasks/datelabel) untuk tier skala waktu. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Mengatur flag yang menentukan apakah label tanggal harus dirender pada setiap halaman ketika periode waktu meluas ke beberapa halaman. Jika nilai 'true', ketika periode waktu meluas ke beberapa halaman, label tanggal untuk periode tersebut dirender pada setiap halaman. Jika nilai 'false', label tanggal hanya dirender sekali sesuai nilai properti `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)).

--------------------

Tidak memiliki padanan di MS Project.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | flag yang menentukan apakah label tanggal harus dirender pada setiap halaman ketika periode waktu meluas ke beberapa halaman. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Mengatur nilai yang menunjukkan apakah menampilkan tanda tick yang memisahkan periode waktu dalam tier.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menampilkan tanda centang yang memisahkan periode waktu dalam tier. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Mengatur unit skala waktu [TimescaleUnit](../../com.aspose.tasks/timescaleunit) untuk tier skala waktu. Nilai default adalah [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | unit skala waktu [TimescaleUnit](../../com.aspose.tasks/timescaleunit) untuk tier skala waktu. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Mengatur nilai yang menunjukkan apakah label tier didasarkan pada tahun fiskal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah label tier didasarkan pada tahun fiskal. |

