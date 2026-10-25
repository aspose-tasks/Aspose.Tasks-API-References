---
title: "ProgressLines"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili garis kemajuan dalam tampilan Gantt Chart."
type: docs
weight: 219
url: /id/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

Mewakili garis kemajuan dalam tampilan Gantt Chart.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | Mendapatkan tanggal untuk menampilkan garis kemajuan mulai. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan sejak tanggal mulai proyek. |
| [getDateFormat()](#getDateFormat--) | Mendapatkan format tanggal ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal saat ini. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada interval berulang. |
| [getDisplaySelected()](#getDisplaySelected--) | Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal yang dipilih. |
| [getFont()](#getFont--) | Mendapatkan font yang digunakan untuk label garis kemajuan. |
| [getLineColor()](#getLineColor--) | Mendapatkan warna garis untuk garis kemajuan saat ini. |
| [getLinePattern()](#getLinePattern--) | Mendapatkan pola garis dari garis kemajuan saat ini. |
| [getOtherLineColor()](#getOtherLineColor--) | Mendapatkan warna garis kemajuan lainnya. |
| [getOtherLinePattern()](#getOtherLinePattern--) | Mendapatkan pola garis untuk garis kemajuan lainnya. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | Mendapatkan warna titik kemajuan lainnya. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | Mendapatkan bentuk titik kemajuan dari garis kemajuan lainnya. |
| [getProgressPointColor()](#getProgressPointColor--) | Mendapatkan warna titik kemajuan. |
| [getProgressPointShape()](#getProgressPointShape--) | Mendapatkan bentuk titik kemajuan. |
| [getRecurringInterval()](#getRecurringInterval--) | Mendapatkan interval berulang. |
| [getSelectedDates()](#getSelectedDates--) | Mendapatkan daftar tanggal yang dipilih untuk menampilkan garis kemajuan. |
| [getShowDate()](#getShowDate--) | Mendapatkan nilai yang menunjukkan apakah akan menampilkan tanggal untuk setiap garis kemajuan. |
| [isBaselinePlan()](#isBaselinePlan--) | Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan untuk rencana dasar atau aktual. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan untuk rencana dasar atau aktual. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | Mengatur tanggal untuk menampilkan garis kemajuan mulai dari. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan sejak tanggal mulai proyek. |
| [setDateFormat(int value)](#setDateFormat-int-) | Mengatur format tanggal ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal saat ini. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada interval berulang. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal yang dipilih. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Mengatur font yang digunakan untuk label garis kemajuan. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | Mengatur warna garis untuk garis kemajuan saat ini. |
| [setLinePattern(int value)](#setLinePattern-int-) | Mengatur pola garis dari garis kemajuan saat ini. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | Mengatur warna garis kemajuan lainnya. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | Mengatur pola garis untuk garis kemajuan lainnya. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | Mengatur warna titik kemajuan lainnya. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | Mengatur bentuk titik kemajuan dari garis kemajuan lainnya. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | Mengatur warna titik kemajuan. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | Mengatur bentuk titik kemajuan. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | Mengatur interval berulang. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | Mengatur nilai yang menunjukkan apakah menampilkan tanggal untuk setiap garis kemajuan. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


Mendapatkan tanggal untuk menampilkan garis kemajuan mulai.

**Returns:**
java.util.Date - tanggal untuk menampilkan garis kemajuan mulai dari.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan sejak tanggal mulai proyek.

**Returns:**
boolean - nilai yang menunjukkan apakah menampilkan garis kemajuan sejak awal tanggal mulai proyek.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Mendapatkan format tanggal ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - format tanggal ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal saat ini.

**Returns:**
boolean - nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal saat ini.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada interval berulang.

**Returns:**
boolean - nilai yang menunjukkan apakah menampilkan garis kemajuan pada interval berulang.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal yang dipilih.

**Returns:**
boolean - nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal yang dipilih.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Mendapatkan font yang digunakan untuk label garis kemajuan.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


Mendapatkan warna garis untuk garis kemajuan saat ini.

**Returns:**
java.awt.Color - warna garis untuk garis kemajuan saat ini.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


Mendapatkan pola garis dari garis kemajuan saat ini. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\\#setLinePattern-int-)).

**Returns:**
int - pola garis dari garis kemajuan saat ini.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


Mendapatkan warna garis kemajuan lainnya.

**Returns:**
java.awt.Color - warna garis kemajuan lainnya.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


Mendapatkan pola garis untuk garis kemajuan lainnya.

**Returns:**
int - pola garis untuk garis kemajuan lainnya.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


Mendapatkan warna titik kemajuan lainnya.

**Returns:**
java.awt.Color - warna titik kemajuan lainnya.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


Mendapatkan bentuk titik kemajuan dari garis kemajuan lainnya.

**Returns:**
int - bentuk titik kemajuan dari garis kemajuan lainnya.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


Mendapatkan warna titik kemajuan.

**Returns:**
java.awt.Color - warna titik kemajuan.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


Mendapatkan bentuk titik kemajuan. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - bentuk titik kemajuan.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


Mendapatkan interval berulang. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


Mendapatkan daftar tanggal yang dipilih untuk menampilkan garis kemajuan.

**Returns:**
java.util.List&lt;java.util.Date&gt; - daftar tanggal terpilih untuk menampilkan garis kemajuan.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


Mendapatkan nilai yang menunjukkan apakah akan menampilkan tanggal untuk setiap garis kemajuan.

**Returns:**
boolean - nilai yang menunjukkan apakah menampilkan tanggal untuk setiap garis kemajuan.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


Mendapatkan nilai yang menunjukkan apakah akan menampilkan garis kemajuan untuk rencana dasar atau aktual.

**Returns:**
boolean - nilai yang menunjukkan apakah menampilkan garis kemajuan untuk rencana dasar atau aktual.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan untuk rencana dasar atau aktual.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menampilkan garis kemajuan untuk rencana dasar atau aktual. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


Mengatur tanggal untuk menampilkan garis kemajuan mulai dari.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal untuk menampilkan garis kemajuan dari. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan sejak tanggal mulai proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menampilkan garis kemajuan sejak tanggal mulai proyek. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Mengatur format tanggal ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | int | format tanggal ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal saat ini. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada interval berulang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menampilkan garis kemajuan pada interval berulang. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menampilkan garis kemajuan pada tanggal yang dipilih.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menampilkan garis kemajuan pada tanggal yang dipilih. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Mengatur font yang digunakan untuk label garis kemajuan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | font yang digunakan untuk label garis kemajuan. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


Mengatur warna garis untuk garis kemajuan saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna garis untuk garis kemajuan saat ini. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


Mengatur pola garis untuk garis kemajuan saat ini. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | pola garis untuk garis kemajuan saat ini. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


Mengatur warna garis kemajuan lainnya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna garis kemajuan lainnya. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


Mengatur pola garis untuk garis kemajuan lainnya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | pola garis untuk garis kemajuan lainnya. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


Mengatur warna titik kemajuan lainnya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna titik kemajuan lainnya. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


Mengatur bentuk titik kemajuan dari garis kemajuan lainnya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bentuk titik kemajuan pada garis kemajuan lainnya. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


Mengatur warna titik kemajuan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color | warna titik kemajuan. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


Mengatur bentuk titik kemajuan. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bentuk titik kemajuan. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


Mengatur interval berulang. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | interval berulang. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


Mengatur nilai yang menunjukkan apakah menampilkan tanggal untuk setiap garis kemajuan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menampilkan tanggal untuk setiap baris kemajuan. |

